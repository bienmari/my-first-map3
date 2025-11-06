# " stuff i do "

!["Bike The Bay" App](img/STUFF_I_DO.png)

## What did I build?

["Stuff I Do"](https://bienmari.github.io/my-first-map3/) For this, you can zoom in and zoom out and click at 3 certain places. I've been over this summer the most because they were the only ones I was at every day you can see sf and oakland and other citys i been to 2 city oakland and san leandro you can see those i and zoom in here its located

!["Bike The Bay" App](img/carbon.png)
this code i reallt like that is the main characters because its where i worked all summer and i  wanted to talk more about it becasue  anyone can look at it and they can see a place to vist when ever they need ideas to check out a small shop to go eat eat.
Exaggerating the elevation profile makes the map more exciting.



Here's a demo:

<img src="img/demo.gif" alt="GIF demo showing how a user can toggle through various maps and view the detailed itinerary" width="300"/>

## Why did I build this?

When I decided to take a group of high school students on 5 bike rides in 5 days, I started wondering how I could communicate the ride itineraries to students (and families/guardians) in an accessible way. 

I set these goals for my product:

1. Families/guardians should **have detailed knowledge** of higher-risk student activities.
2. Students should **practice engaging** with visualized spatial data to **independently answer their own questions** about each day's ride location, duration, elevation, Points of Interest, or itinerary.

## Tech stack

To build this app, I used the following tools:

1. [Google Maps](https://www.google.com/maps), I used google maps to get the cordantes of the places where i have gone over the summer.
2. [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/guides) i used mapbox to get the custamastion for my map and what we used to create my map. 
3. [Visual Studio Code](https://code.visualstudio.com/download) this is where im working on my code right now.
4. [GitHub pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site),  that where i have my map and my code and my first map

## Feature Spotlight

One key feature I want to spotlight is the exaggerated terrain. 

If you look closely at the map, you might notice that the hills and mountains are very pronounced. That's because I exaggerated the apperance of topography by 250%. Here's how I did it:

Following [this example](https://docs.mapbox.com/mapbox-gl-js/example/add-terrain/), I first added [this](https://docs.mapbox.com/data/tilesets/reference/mapbox-terrain-dem-v1) Mapbox raster tileset `mapbox://mapbox.mapbox-terrain-dem-v1` to the map as a source. This tileset contains a Digital Elevation Model (DEM) encoded in the RGB values. So, by using `.setTerrain`, we can use the elevation values in the tileset to enable topographical extrusion – to make the map 3D!

So, why 250%? Well, what's the point of adding subtle (realistic) terrain, when my goal is to **prepare students to face some aggressive climbs**? _Those hills should look as mean as they feel._

Check it out:

![terrain eggageration code](img/terrain-code.png)

<img src="img/demo-3d-terrain.gif" alt="GIF demo showing 3d terrain" />

_Exaggerating the elevation profile makes the map more exciting._

## Contributions

Feel free to copy the code if you want it! Comments are welcome on [this blog post](https://domlet.github.io/posts/bike-the-bay/).
