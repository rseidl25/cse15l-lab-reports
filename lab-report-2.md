# Servers and Bugs
#### Written by: Ryan Seidl *(Wed. 3pm, B260)*
---
## *Part 1:* StringServer
For this part, I wrote a web server program **StringServer** that displays a list of strings that the user is able to add through URL requests. **StringServer** uses the prewritten **Server.java** file from Lab 2 in order to be hosted as a web server.

Below is the code for the **StringServer** program:

```
  import java.io.IOException;
  import java.net.URI;
  import java.util.ArrayList;

class Handler implements URLHandler {

    ArrayList<String> stringList = new ArrayList<String>();

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {

            String output = "";
            for(int i=0; i<stringList.size(); i++)
                output += stringList.get(i) + "\r\n";
            
            return output;

        }else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {

                    stringList.add(parameters[1]);

                    String output = "";
                    for(int i=0; i<stringList.size(); i++)
                        output += stringList.get(i) + "\r\n";

                    return output;
                }
            }

            return "404 Not Found!";

        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```

> `StringServer.java` consists of two classes: `StringServer` and `Handler`. The former of the two handles the creation of the web server, while the latter handles the function of the web server.

The following are two demos of `StringServer` as well as their corresponding explanations:

![Image](ssEx1.png)
#### Example 1: `/add-message?s=Hello`
* The method called in this example is `handleRequest`.
* In this case, the relevant argument for the method is `/add-message?s=Hello`, which fulfills the parameter `URI url`. The relevant field of the class is `stringList`, which holds each string that the user inputs in the URL request. The value of `stringList` is now `Hello` because the method `handleRequest` added the String `Hello` to `stringList`.
* The field `stringList` changed from being empty to containing the String, `Hello`.

![Image](ssEx2.png)
#### Example 2: `/add-message?s=How are you?`
* Similarly to example 1, the method called in this example is `handleRequest`.
* This time, the relevant argument for the method is `/add-message?s=How are you?`, which again fulfills the parameter `URI url`. The relevant field of the class is also `stringList`. This time, however, it contains `Hello` at index 0 and `How are you?` at index 1 because the method `handleRequest` added the String `How are you?` to `stringList`.
* The field `stringList` changed from containing only `Hello` to containing the two Strings, `Hello` and `How are you?`.

---
## *Part 2:* Bug Fixing
In this part, I will be analyzing a bug in the `ReverseInPlace` method in `ArrayExamples.java`.

**Failure-inducing input:**
```
  @Test
  public void testReverseInPlaceMultipleValues(){

    int[] multipleValueInput = {10, 8, 6, 4, 2, 0};
    ArrayExamples.reverseInPlace(multipleValueInput);
    assertArrayEquals(new int[]{0, 2, 4, 6, 8, 10}, multipleValueInput);
    
  }
```

**Working input:**
```
  @Test
  public void testReverseInPlaceMultipleValues(){

    int[] multipleValueInput = {10, 8, 6, 4, 2, 0};
    ArrayExamples.reverseInPlace(multipleValueInput);
    assertArrayEquals(new int[]{0, 2, 4, 6, 8, 10}, multipleValueInput);
    
  }
```

**Failure-inducing input:**
```
  @Test
  public void testReverseInPlaceMultipleValues(){

    int[] multipleValueInput = {10, 8, 6, 4, 2, 0};
    ArrayExamples.reverseInPlace(multipleValueInput);
    assertArrayEquals(new int[]{0, 2, 4, 6, 8, 10}, multipleValueInput);
    
  }
```

**Failure-inducing input:**
```
  @Test
  public void testReverseInPlaceMultipleValues(){

    int[] multipleValueInput = {10, 8, 6, 4, 2, 0};
    ArrayExamples.reverseInPlace(multipleValueInput);
    assertArrayEquals(new int[]{0, 2, 4, 6, 8, 10}, multipleValueInput);
    
  }
```
