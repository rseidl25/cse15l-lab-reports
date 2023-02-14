# `grep` Command Options
#### Written by: Ryan Seidl *(Wed. 3pm, B260)*
##### *Standard Syntax:* `grep [OPTION] pattern [FILE]`
---
### Option 1: `-w`
#### Returns lines containing the *exact* matched word

➡️**Example 1:**

Input: 

```
grep -w "cross" skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

Output: 

```
Start at the bridge. The city has more than one, but the one is, of course, the Golden Gate Bridge. The name Golden Gate was given to the city’s harbor entrance in 1846 by Captain John Frémont, but the mile-wide channel lay unspanned until the bridge, a masterpiece of engineering by Joseph Strauss, was completed in 1937. At 4,200 ft (1,280 m), it was the world’s longest single span until New York’s Verrazano Narrows Bridge surpassed it in 1964, but few would deny that it remains the most beautiful suspension bridge in the world. It took four years and $35 million to build; more than 40 million vehicles now cross over the span every year. You can take a bus to the bridge entrance and then walk across — it’s just as exciting an urban adventure as climbing up the Eiffel Tower or the Empire State Building. The bridge trembles underneath your feet, and the lamp-posts rattle as the wind whistles through swooping cables. But don’t worry — the 746-ft- (227-m-) high towers are well embedded in earthquake-proof foundations.
Once you’ve bought your copy of On the Road, cross Jack Kerouac Street and settle down with your purchase over a drink at Vesuvio’s, another famous literary hangout. Or if it’s a sunny day, buy a sandwich from a delicatessen and enjoy a picnic on Washington Square, a splash of green overlooked by the white spires of the Church of Saints Peter and Paul, where Marilyn Monroe and Joe DiMaggio were married in 1954.
Don’t be put off by the name Death Valley. It is a legacy of the bitter hardships endured by Gold Rush hopefuls who set out to cross the desert from Arizona and Nevada. Some never made it. Today’s travelers, however, are well catered to, with motels and campsites at Furnace Creek and Stovepipe Wells. Begin at the Furnace Creek Visitor Center, where you can pick up maps and information on the road conditions, hiking trails, and general desert safety. Driving is the only way to get around, but remember that distances are great and gasoline stations few and far between. Make sure your car is in good mechanical condition and that the tank is full before you begin each day’s tour. Also, you would be well advised to carry spare water, just in case the radiator boils over.
```

Explanation:
> This command searches through the `California-WhereToGo.txt` file and returns 3 lines, each containing the exact word *"cross"*.
> Since some words contain other words (*"across"* containts *"cross"*), this option is useful if you're searching for information regarding 
> an exact word within a `.txt` file.


➡️**Example 2:**

Input: 

```
grep -w "no" skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

Output: 

```
A 12-acre (4.8-hectare) rock with no cultivable soil, all the earth and water for the shrubs and trees here had to be shipped in by the US Army, for whom it had been a “disciplinary barracks” until 1934. Separated from mainland San Francisco by 11⁄2 miles (2.4 km) of treacherous, ice-cold water, haunted by sharks and dangerous currents, it was the ideal location for America’s most notorious federal penitentiary. However, it proved enormously expensive to run, and was closed down in 1963.
The roller-coaster dips and crests of the city’s hills, breaking up the monotony of the standard grid system of streets, reach a crazy climax on Lombard Street between Hyde and Leavenworth. After you’ve negotiated all eight hairpin bends lined with gardens of hydrangeas, you’re not going to quibble about the claim that it’s the “crookedest street in the world.” Two blocks south is Filbert Street, boasting the steepest slope — a stomach-churning 31.5 percent gradient, with no bends.
You can drive to the vineyards from San Francisco via Interstate 80, across the Bay Bridge, but bus tours are also available through the major providers. You can also arrange a custom tour, visiting wineries of your choice, through Wine Country Jeep Tours (Tel. 800/539-5337, toll-free in US). The Napa Valley Wine Train is another option for a scenic hands-off chug through the valley, including lunch or dinner, but no winery visits.
Beside the Plaza is Monterey’s Fisherman’s Wharf. Like San Francisco’s, it is a collection of souvenir shops and restaurants on the dock, offering a great view across the boats in the marina. The fish on sale is most definitely fresh, but alas, no longer abundant enough to keep Cannery Row going as more than a weather-beaten curiosity. The famous sardine fisheries finally closed down in the 1940s as a result of over-fishing, but the waterfront district of timbered canneries, immortalized by the novelist John Steinbeck as “a poem, a stink, a grating noise, a quality of light, a tone, a habit, a nostalgia,” has found a new lease on life today as a tourist attraction with souvenir shops, delightful cozy boutiques, and artists’ studios.
A combination of engineering genius and shady business deals brought water hundreds of miles across mountains and desert to slake the city’s thirst and nurture its lush gardens and palm trees. An abundance of space then allowed the city to sprawl, but distance was no problem — cheap oil and the car produced a vast freeway system, which links the coast, the hills, and the farthest-flung valleys in one huge metropolitan region. Visitors flying into L.A. at night get a grand view of the network of traffic arteries, with cars and trucks surging along like blood corpuscles pumping through the veins of some living organism.
“The beach,” as locals refer to it, stretches some 72 miles (115 km) from Malibu, through Santa Monica, Venice, Marina del Rey, Hermosa, and Redondo to Palos Verdes, before the white sands run into the pollution around the San Pedro and Long Beach shipyards. There’s no better way to get the special feel of Los Angeles than by heading right down to the beach, because in L.A. the beach is not just for holidays and weekends — it’s a year-round playground, community center, gymnasium, solarium, and singles bar.
Another beautiful walk, and by no means an exhausting one, is out to Crescent Meadow, passing on the way such venerable trees as the Bear’s Bathtub, the Shattered Giant, and the Chimney.
Of all the wonders of California, the high desert is perhaps the greatest surprise. The desert is no monotonous expanse of sand dunes, but a beautiful, variegated land full of color and space. In summer it is a bizarre landscape of jagged rock and gravel, naked mountains and salt lakes, baked and shimmering in the desert heat. Go in winter and you may see drifts of spring flowers blooming in the wake of the sparse rains that make it over the snow-dusted Panamint Mountains in the west. Unhidden by vegetation, the colors of the rocks — brick red, ochre, green, and purple-brown — are dramatically deepened at sunset and dawn, creating unforgettable views.
If it’s the traditional Las Vegas you dream of, the best time to arrive is at sunset, when the city lights loom out of the desert darkness. For the same reason, nighttime is the best time to roam along The Strip, when the lights are brightest and the tables at their liveliest. Apart from the décor, the casinos are pretty much alike — admission is free, and they’re open 24 hours a day, 365 days a year. There are one-armed bandits (slot machines) near the doors, the delights of roulette, blackjack, craps, and Keno further in, and everywhere huge television screens showing horse-racing and other big sporting events from all over the country. For the bewildered, there are free booklets explaining how best to lose your money at the various tables, and free blackjack lessons in the afternoons. You will notice there are no clocks or windows in the casinos — the management wants you to lose track of time.
```

Explanation:
> Here, `grep -w` is used on the same `.txt` file, but instead it returns each of the 9 lines containing the word *"no"*.
> Given that searching for *"no"* without the `-w` flag returns 84 lines instead of 9, this flag is extremely useful when
> looking for an exact word in a long `.txt` file.

#### Sources Used
* I used the `grep` manual by typing `grep --help` in the VSCode terminal.
* https://www.geeksforgeeks.org/grep-command-in-unixlinux/
* https://www.makeuseof.com/grep-command-practical-examples/

---
### Option 2: `-R`
#### Performs a *recursive* search through all *subdirectories*

➡️**Example 1:**

Input: 

```
grep -R "Big Sur" skill-demo1-data/
```

Output: 

```
skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt:The coastal highway south from Carmel to Big Sur is only 30 miles (48 km) long, but it takes more than an hour of careful driving. Squeezed in between the Pacific and the Santa Lucia mountains, the road twists and turns along a quite narrow ledge hacked out high above the pounding surf, with spectacular bridges spanning the deep canyons.
skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt:The numerous state parks along the Big Sur coast offer marvelous opportunities for outdoor activities like camping, hiking, and fishing. The writer Henry Miller made his home here during the 1950s and 60s, and communities of artists continue to live in cabins in the woods and canyons.
```

Explanation:
> This command searches through every file in every subdirectory of `skill-demo1-data/` and returns the lines in
> `.txt` files where the string *"Big Sur"* is contained. This command is useful because it provides a quick way to check
> if a certain directory contains information on a certain subject in any of its subdirectories.

➡️**Example 2:**

Input: 

```
grep -R "Hollywood" skill-demo1-data/written_2/non-fiction/
```

Output: 

```
skill-demo1-data/written_2/non-fiction/OUP/Castro/chM.txt:In the last thirty years Mariachi festivals have become very popular throughout the Southwest. They have been held in San Antonio, Texas; Tucson, Arizona; San Jose, California; and even Universal Studios in Hollywood originated a festival in 1985. Los Angeles is home to the largest assemblage of Mariachi musicians in the United States.
skill-demo1-data/written_2/non-fiction/OUP/Castro/chR.txt:The Texas Rangers, known by Tejanos as Los Rinches, probably a Spanish pronunciation of “ranger,” became notorious within Chicano communities because of their brutality. Established in 1835, right before Texas’s independence from Mexico in 1836, the Texas Rangers were viewed as a state militia. They were actually organized by Stephen F. Austin, who hired the first ten in 1823 to wage war against Indians. Often portrayed as heroic figures, protectors of law and order, by Hollywood and in literature, Los Rinches were greatly feared and hated by Texas Mexicans. During the U.S.-Mexican War they led the way for General Zachary Taylor’s march to Monterrey, Mexico.
skill-demo1-data/written_2/non-fiction/OUP/Castro/chV.txt:The vaquero was the early Hispano cowboy and the antecedent of the Hollywood cowboy. Horses and cattle were brought to New Spain by the Spaniards. When Hernán Cortés landed on the eastern shore of Mexico, he had with him sixteen horses and at least three breeds of cattle. Cattle breeding was a tradition hundreds of years old in Spain, and Cortés brought this tradition to Mexico and eventually to the Southwest. The Spaniards introduced the system of el rancho, with vaqueros being the workers who herded the cattle and conducting cattle drives. Vaca means “cow” and a vaquero is “one who works with cows.” The Spanish mission padres recognized this labor and conscripted mestizos (mixed-race people), Indians, and Mexicans to take care of the cattle. It was these individuals who developed the system, equipment, practices, and traditions that have lasted these past few hundred years. The Anglo cowboy learned everything about cattle from the vaquero. 
skill-demo1-data/written_2/non-fiction/OUP/Castro/chV.txt:The Mexican vaquero was a laborer, a peon who was used by the missionaries to ride the horses and take care of the cattle. So it was the culture of the vaquero that became the basis for the romantic cowboy of Hollywood. The ensemble, equipment, and clothing of the vaquero evolved through the years as a combination of Spanish leather and regional indigenous fabrics. He always wore a sombrero with a wide brim, a leather chaqueta (jacket), tight-fitting knee-length sotas (breeches), and botas (leather leggings) for protection. The vaquero also wore iron spurs, like those worn by the Conquistadores, which are still worn to this day. The various styles of saddles, from the Moorish to the Spanish war saddle, eventually changed when the vaqueros began making their own saddles, more suitable for riding hard and for quick mounting and dismounting.
skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch3.txt:Gehry’s talent is his exceptional formal imagination; his skill as an architect is to reconcile the forms he imagines with the functional demands of his client. And, of course, to find ways to build those forms. This is generally done without fuss. The titanium sheets simply follow the churning surfaces like shingles on a Shingle Style roof; limestone is used in a similarly unaffected fashion, without articulated joints. Gehry shares a minimalist approach to details with the early architects of the International Style, but he deploys these details to different ends. By removing familiar elements such as coping strips, fascias, and trim, he accentuates the sculptural quality of his buildings. There are no roofs or walls or windows in the Guggenheim, there are only swirling and twisting planes of metal, stone, and glass. An architecture critic once described Gehry as “a smart man from Hollywood,” which nicely captures the architect’s blend of exuberant showmanship and canny behind-the-scenes savvy.
```

Explanation:
> Similar to example 1, this command searches through all the subdirectories in `skill-demo1-data/written_2/non-fiction/`,
> and returns the lines in `.txt` files containing the string *"Hollywood"*. The `-R` option is useful because it saves a lot
> of time that the user would otherwise spend using the `grep` command on every single subdirectory.


#### Sources Used
* I used the `grep` manual by typing `grep --help` in the VSCode terminal.
* https://www.geeksforgeeks.org/grep-command-in-unixlinux/

---
### Option 3: `-n`
#### Returns *matched lines* and their respective *line numbers*

➡️**Example 1:**

Input: 

```
grep -n "Big Sur" skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

Output: 

```
72:The coastal highway south from Carmel to Big Sur is only 30 miles (48 km) long, but it takes more than an hour of careful driving. Squeezed in between the Pacific and the Santa Lucia mountains, the road twists and turns along a quite narrow ledge hacked out high above the pounding surf, with spectacular bridges spanning the deep canyons.
73:The numerous state parks along the Big Sur coast offer marvelous opportunities for outdoor activities like camping, hiking, and fishing. The writer Henry Miller made his home here during the 1950s and 60s, and communities of artists continue to live in cabins in the woods and canyons.
```

Explanation:
> This command searches the `California-WhereToGo.txt` file and returns the text and line numbers of the lines
> that contain the string *"Big Sur"*. If multiple lines around the same number are returned by this command, it's
> useful in showing where information about a certain subject is most prominent in a given file.

➡️**Example 2:**

Input: 

```
grep -n "Ocean" skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

Output: 

```
47:The western end of the park boasts two turn-of-the-century windmills that overlook the surf at Ocean Beach. Chilly water and dangerous currents make this more a beach for strollers, sunbathers, and experienced surfers — swimming is sternly discouraged. The northern end of the beach is overlooked by the Cliff House. The present building was built in 1909 and now houses restaurants serving breakfast, lunch, and dinner (the food isn’t highly recommended), a bar (drinks at sunset are a better idea), and the Musée Mécanique, one of the largest privately owned collections of old-fashioned coin-operated arcade novelties in the world. Admission is free, but a pocketful of quarters will be useful. There is also a fine view of Seal Rocks and, on a clear day, you can see as far as the Farallon Islands, lying 30 miles (48 km) offshore.
70:The 17-Mile Drive is a lovely scenic toll road starting at Lighthouse Avenue in Pacific Grove, a pleasant waterside town of Victorian houses and clapboard cottages a few miles beyond Monterey. The drive passes through beautiful cypress groves along a wild and rocky coastline, where you can watch birds, otters, and sea lions in the wild, before passing through the famous golf courses at Pebble Beach and finally reaching the exclusive resort town of Carmel-by-the-Sea, famous for once having Clint Eastwood as mayor. It is a quaint, picture-postcard village full of kitschy cottages, with narrow, tree-lined streets crammed with expensive restaurants, art galleries, and craft shops. At the foot of Ocean Avenue lies the beautiful white sand of Carmel Beach, backed by shady pines and cypress trees. Southeast of the town is the peaceful Carmel Mission, where Father Junípero Serra himself lies buried.
```

Explanation:
> This command checks the same `.txt` file as example 1, but instead returns the text and line numbers of the lines
> containing the string *"Ocean"*. This command is useful when you want to find information about a certain subject but
> don't want to read through the entire `.txt` file because you'll be presented with information on the exact line number.

#### Sources Used
* I used the `grep` manual by typing `grep --help` in the VSCode terminal.
* https://www.geeksforgeeks.org/grep-command-in-unixlinux/

---
### Option 4: `-i`
#### Ignores *case* when finding matches

➡️**Example 1:**

Input: 

```
grep -i "ocean" skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

Output: 

```
San Franciscans are quite unashamedly in love with their town. Its natural setting, nestled in the hills around the bay, makes the city uncommonly cozy; the zip in the air is invigorating, and even the fog that rolls in off the ocean seems more romantic than chilling. If you have a car, one way to begin your visit is to travel along 49-Mile Drive, which provides a comprehensive tour of the main sights. You’ll need to use a good map, as the blue signposts with a white seagull in the center can be difficult to locate. Stop off at Twin Peaks (the road to get there starts near the southern end of Market Street) for an excellent panoramic view of the city and the bay, then park the car, put on a pair of comfortable walking shoes, and take to the city’s first-class public transport system (see page 120).
The western end of the park boasts two turn-of-the-century windmills that overlook the surf at Ocean Beach. Chilly water and dangerous currents make this more a beach for strollers, sunbathers, and experienced surfers — swimming is sternly discouraged. The northern end of the beach is overlooked by the Cliff House. The present building was built in 1909 and now houses restaurants serving breakfast, lunch, and dinner (the food isn’t highly recommended), a bar (drinks at sunset are a better idea), and the Musée Mécanique, one of the largest privately owned collections of old-fashioned coin-operated arcade novelties in the world. Admission is free, but a pocketful of quarters will be useful. There is also a fine view of Seal Rocks and, on a clear day, you can see as far as the Farallon Islands, lying 30 miles (48 km) offshore.
The 17-Mile Drive is a lovely scenic toll road starting at Lighthouse Avenue in Pacific Grove, a pleasant waterside town of Victorian houses and clapboard cottages a few miles beyond Monterey. The drive passes through beautiful cypress groves along a wild and rocky coastline, where you can watch birds, otters, and sea lions in the wild, before passing through the famous golf courses at Pebble Beach and finally reaching the exclusive resort town of Carmel-by-the-Sea, famous for once having Clint Eastwood as mayor. It is a quaint, picture-postcard village full of kitschy cottages, with narrow, tree-lined streets crammed with expensive restaurants, art galleries, and craft shops. At the foot of Ocean Avenue lies the beautiful white sand of Carmel Beach, backed by shady pines and cypress trees. Southeast of the town is the peaceful Carmel Mission, where Father Junípero Serra himself lies buried.
At Point Lobos State Reserve you can hike right down to the ocean’s edge. Watch especially for the playful sea otters, which can often be seen floating on their backs munching on a juicy abalone or two. From December to March, look out also for pods of migrating gray whales.
At Nepenthe, Orson Welles built a honeymoon cottage for Rita Hayworth in the days when film stars did the romantic things expected of them by their adoring public. Now it has been expanded and converted into a restaurant, well worth a visit for its incomparable view of the ocean.
Long Beach — which is 7 miles (11 km) long, in fact — is the last resting place of one of the world’s biggest ever cruise ships, the Queen Mary, a nostalgic reminder of the grand era of luxury ocean liners. Since being moored here in 1967, the Queen Mary’s staterooms have been turned into a hotel, and her dining rooms into a restaurant; the rest of the ship is open to the public with self-guided tours (admission is free). Launched on the River Clyde in Scotland in 1936 for the Cunard line, the Queen Mary is 1,019 ft (310 m) long, displaces 81,237 tons, and carried a complement of 1,174 officers and crew, with accommodation for 1,959 passengers. Firework displays are staged over her on Friday and Saturday nights during summer.
San Diego’s beaches are truly beautiful and remarkably unspoiled, stretching for some 27 miles (43 km) up to the elegant suburb of La Jolla (pronounced “la HOY-a,” Spanish for “jewel”), whose centerpiece is the tiny rock basin of La Jolla Cove. The rocky coast to the south is marvelous for walking, and away from the ocean there are stylish shops and elegant restaurants to visit. The marine life of southern California is splendidly displayed in the Birch Aquarium at Scripps, which is spectacularly sited on the hilltop above La Jolla. 
```

Explanation:
> This command searches the `California-WhereToGo.txt` file for the word *"ocean"*, disregarding `case`. In this case,
> the `.txt` file refers to the ocean itself as well as Ocean Beach, so using the `-i` option returns all of the 
> lines that contain the word.

➡️**Example 2:**

Input: 

```
grep -i "Water" skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt
```

Output: 

```
San Franciscans are quite unashamedly in love with their town. Its natural setting, nestled in the hills around the bay, makes the city uncommonly cozy; the zip in the air is invigorating, and even the fog that rolls in off the ocean seems more romantic than chilling. If you have a car, one way to begin your visit is to travel along 49-Mile Drive, which provides a comprehensive tour of the main sights. You’ll need to use a good map, as the blue signposts with a white seagull in the center can be difficult to locate. Stop off at Twin Peaks (the road to get there starts near the southern end of Market Street) for an excellent panoramic view of the city and the bay, then park the car, put on a pair of comfortable walking shoes, and take to the city’s first-class public transport system (see page 120).
Start at the bridge. The city has more than one, but the one is, of course, the Golden Gate Bridge. The name Golden Gate was given to the city’s harbor entrance in 1846 by Captain John Frémont, but the mile-wide channel lay unspanned until the bridge, a masterpiece of engineering by Joseph Strauss, was completed in 1937. At 4,200 ft (1,280 m), it was the world’s longest single span until New York’s Verrazano Narrows Bridge surpassed it in 1964, but few would deny that it remains the most beautiful suspension bridge in the world. It took four years and $35 million to build; more than 40 million vehicles now cross over the span every year. You can take a bus to the bridge entrance and then walk across — it’s just as exciting an urban adventure as climbing up the Eiffel Tower or the Empire State Building. The bridge trembles underneath your feet, and the lamp-posts rattle as the wind whistles through swooping cables. But don’t worry — the 746-ft- (227-m-) high towers are well embedded in earthquake-proof foundations.
Visible in the distance is the San Francisco–Oakland Bay Bridge, known locally as just the Bay Bridge. This silver-gray structure swings across to Oakland via two suspension spans, a cantilever span, and a tunnel through Treasure Island. It’s the bridge you’ll take to go to Berkeley (see page 40) and is one of the routes to the wine country of Napa and Sonoma (see page 41).
Of the many cruises you can take on San Francisco Bay, the most entertaining is a trip to the abandoned prison island of Alcatraz. The name is a distortion of the Spanish Isla de Alcatraces (Pelican Island). National Park Rangers offer informative and witty self-guided audio tours around the former home of Al Capone as well as other convicts such as Robert Stroud, the famous “Birdman of Alcatraz.”
It is worth climbing to the top of Telegraph Hill for the view of the bay from the top of Coit Tower, built in 1934 to honor the city’s fire department. One of San Francisco’s many landmarks, its shape is not meant to resemble the nozzle of a fire hose, as is so often reported. Inside you will find Socialist Realist murals depicting “Life in California, 1934.” Take a look at the cottages and gardens around the Greenwich Steps, clinging to the steep slope overlooking the bay — this is one of the city’s most desirable addresses.
Head down to Montgomery Street, the heart of San Francisco’s financial district, also known as the “Wall Street of the West.” This area was founded on the profits of the 1849 Gold Rush (see page 16), and is now bristling with skyscrapers of chrome and glass. Take a look at the Old Coin and Gold Exhibit at the Bank of California (400 California Street), with its collection of gold coins and currency, or the Wells Fargo History Room in the Wells Fargo Bank (420 Montgomery Street), which displays Gold Rush memorabilia, including one of the original Wells Fargo stagecoaches. You’re not likely to miss the Transamerica Pyramid, a 853-ft- (256-m-) tall building with a 212-ft (64-m) spike, at the corner of Montgomery and Washington. It’s one of those buildings that purists start off hating because it clashes with the “spirit” of San Francisco, and then defend in the next generation as the very epitome of its age. If it’s time for lunch or dinner, head to Belden Alley (between Bush, Pine, Kearny, and Montgomery streets), where you’ll find an entire block of excellent restaurants, all with outdoor seating
The highway continues on to Point Reyes National Seashore, a large wilderness park on the coast, complete with beautiful rolling hills, sandy bays, and exciting wild surf. Find maps and hiking recommendations at the Bear Valley Visitor Center. Explore the bird-haunted lagoon at Drake’s Bay, a peaceful cove where Francis Drake claimed California for England in 1579, or hike your way through the Earthquake Trail, a path that follows the San Andreas Fault. The tiny burg of Point Reyes Station across the little bridge on Petaluma Road contains some good restaurants and an excellent spot for gourmet take-out, Tomales Bay Foods on Fourth Street.
Take the BART subway from Market Street or drive across the Bay Bridge to make a pilgrimage to the University of California campus at Berkeley (pronounced BIRK-lee), the scene of 1960s student radicalism. Opened in 1873, Berkeley is the oldest of the University of California’s nine campuses. Tours of the museums, library, gardens, and other sights are organized from the Student Union at the end of Telegraph Avenue (Monday–Saturday at 10am). The free and easy access to the university’s facilities will give you an insight into Berkeley’s open personality. The nearby streets are lined with lively cafés and interesting bookshops. If you’re driving, head over to Fourth Street for good food and prodigious shopping and people-watching.
The coastal highway south from Carmel to Big Sur is only 30 miles (48 km) long, but it takes more than an hour of careful driving. Squeezed in between the Pacific and the Santa Lucia mountains, the road twists and turns along a quite narrow ledge hacked out high above the pounding surf, with spectacular bridges spanning the deep canyons.
Beyond San Simeon the rugged coastline begins to relent, and farms and oil rigs take the place of crags and canyons. Rural Route 1 joins the multi-lane US Highway 101 at San Luis Obispo for the final leg to Los Angeles, but two places are worth a detour from the freeway.
On State Street, which runs from the beach up through the center of town, you’ll find a thriving downtown filled with stores, theaters, and restaurants. In particular, take a peek at the Arlington Theater; the inside was designed to mimic a Spanish-style courtyard at dusk, including a star-filled sky. There’s history on display, too, at Mission Santa Barbara (corner of Laguna and Mission streets). The mission, which was founded on 4 December 1786, the Feast of St. Barbara, offers a self-guided tour of its restored church and outbuildings. Also worth a visit is the beautiful Santa Barbara County Courthouse — a magnificent Spanish-Moorish–style edifice dating from 1927.
L.A. covers such an immense area that the first-time visitor can easily feel overwhelmed. The best way to approach the city is to break it down into smaller regions and then take them one at a time — Downtown, Hollywood, Westside, the Coast, the Valleys, and Orange County.
While you’re on the north side of town, take a drive around the Hollywood Hills for a superb view of the city. The classic Los Angeles cruise is along Mulholland Drive. On a clear day you can see Long Beach, 25-miles (40-km) away across the vast, sprawling metropolis.
Rodeo Drive (pronounced Ro-DAY-oh) is the famous shopping street (if you saw the movie Pretty Woman, you’ve seen Rodeo Drive) and it’s just as upscale and sophisticated as advertised. If you’re visiting in the summer or around Christmas, take a half-hour guided tour on the sweet Beverly Hills Trolley for $1. Meet the trolley on the corner of Rodeo and Dayton Way — it’s the only bargain you’ll find in the neighborhood.
One of the most enjoyable is a tour of the film and television studios located in the San Fernando Valley. Two major TV networks — CBS and NBC — welcome you onto their sets for a look behind the scenes at some of America’s most popular TV shows. A limited number of tickets to live shows are available. Universal Studios Hollywood, just north of the Hollywood Freeway (either the Universal Center Drive or the Lankershim Boulevard exits), offers an elaborate tour in open trams. In the course of displays of special-effects trickery you’ll be attacked by the shark from Jaws, meet up with a three-story-tall King Kong, and be subjected to all the earthquakes, floods, and fires you ever saw in a disaster movie. You can also take a look behind the scenes and learn about techniques that are used to create film’s great illusions. The highlight is the Back To The Future ride. Seated in a flight simulator shaped like the famous time-traveling DeLorean car in the films, you will be taken on a hair-raising chase through time and space.
One of the best ways to appreciate San Diego’s sparkling beauty is from the sea. You can take a cruise along the bay — boat trips leave from Harbor Drive, just south of the Maritime Museum — out past the man-made Harbor and Shelter Islands and around the tip of the Coronado peninsula (occupied by a US Naval Air Station — the film Top Gun was set nearby in northern San Diego) to Point Loma out on the Pacific coast. The seemingly endless procession of fishing boats, yachts, and US Navy vessels makes for a fascinating tour.
The highlight of the park is the San Diego Zoo, one of the finest in the world. Established in 1922, the zoo was a pioneer in the use of moats, ravines, rocks, and embankments rather than bars and cages, giving the animals as large, free, and natural a living space as possible. It is famous for its Sumatran tigers and Malaysian sun bears as well as a colony of koala bears — the only breeding population outside Australia. You can enjoy a bird’s-eye view of the zoo from the Skyfari aerial tramway, or take a guided tour bus. An extension of the zoo is located 30 miles (48 km) north at the San Diego Wild Animal Park in Escondido, where 2,500 animals, including zebra, lions, elephants, cheetahs, and rhinoceros, roam freely.
The scenic Yosemite Valley is a perfect example of a glacier-carved canyon, with its sheer granite walls 3,200ft (975m) high plunging to a flat floor of woods and wild-flower meadows, enclosing the waters of the Merced River. Your “base camp” could be a plush hotel room, more modest lodge accommodation, or even just a tent. From the valley meadows you can hike, bike (rentals at Yosemite Lodge or Curry Village), or take the shuttle bus to all the principal sights. 
The crazed and pinnacled surface of the salt-caked lake bed has earned it the nickname of Devil’s Golf Course. Take a walk out across that glaring expanse of baked salt — the atmosphere of desolation is almost exhilarating. If you look closer at the salt under your feet, you’ll discover that the expansion of the crystallizing mineral has heaved it into bizarre funnels, swirls, and other intricate patterns.
At the northern boundary of Death Valley, 52 miles (84 km) from Furnace Creek, lies the remarkable Scotty’s Castle, a luxuriously furnished 1920s Spanish-style mansion that rises improbably from the bed of Grapevine Canyon. It was built for a Chicago millionaire, Albert Johnson, who spent his winters prospecting for gold with his partner and friend, Walter Scott, known to all as “Death Valley Scotty.” Guided tours take you round the lavish interior; you can wander the grounds at will. Nearby lies Ubehebe Crater, the spectacular result of a volcanic explosion. A short trail leads to the floor of the crater.
```

Explanation:
> Similar to example 1, this command ignores case and returns every line in `California-WhereToGo.txt` that
> contains the word *"take"*. Of the 20 lines returned, 4 of them contain the word capitalized at the start 
> of a sentence, so this option is helpful in avoiding this issue when returning an accurate word count.


#### Sources Used
* I used the `grep` manual by typing `grep --help` in the VSCode terminal.
* https://www.geeksforgeeks.org/grep-command-in-unixlinux/

---
