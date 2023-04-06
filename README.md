## About the Project:
This project aims on creating a marker simulation of people moving from one place to another using different modes of transport in the IIT Jodhpur campus. 

We have used the tool “Leaflet” to create this marker simulation i.e., to move each mode of transport from one place to another in the campus via the shortest route possible. Leaflet is an open source Javascript library used to build web mapping applications. A typical use of Leaflet involves binding a Leaflet "map" element to an HTML element.

We searched for numerous other tools for this project which includes ABStreet, SUMO but there were a few issues in them. Leaflet didn’t have any of those which we were facing in the rest, and hence made it the most convenient library for the marker simulation. Leaflet has a few inbuilt functions in it which made it easier for us to figure out how to move the markers. 

## About the files

Moving marker.js - A file which **must** be there for the animation to take place (L.Routing is dependent on this file)

sim.html - In this, one marker is placed on the map based on its lattitude and longitude coordinates entered in the code. The other marker can be selected on our own by clicking another point in the map. The initial marker then sets a route to the place which we have selected and animates itself to the selected final marker.

coordinates.html - The lattitude and the longitude of the marker on the map are displayed as the output. The coordinates of a place can be obtained by clicking on it.

index.html - Assuming there are 2 markers (the initial destination and the final destionation. However the code contains 6 markers, which is 3 trips in total). When the initial marker is clicked, a bouncing animation takes place and then animates itself to the final destionation via a route which is found by the L.Routing function. However, if there are multiple trips, 
**the markers which indicate the initial points of the respective trips must be clicked sequentially** in the order in which they have been written in the code (the second trip cannot start unless the first trip starts).

## Output of the code

The snapshot below shows the 4 different people at 4 different places which are the initial points and the red markers indicate the destination towards which they will be travelling.

<img width="480" alt="Screenshot 2023-04-06 at 14 25 58" src="https://user-images.githubusercontent.com/84466567/230327931-80f5c661-bbdf-438b-87bb-1a458986c868.png">

On clicking each of the icons, they move from their start position to their destinations via the shortest path possible. A snapshot of the vehicles as they are moving is attached below. The instructions to follow while going between 2 different locations appears on the right once the marker starts its journey.

<img width="561" alt="Screenshot 2023-04-06 at 14 29 41" src="https://user-images.githubusercontent.com/84466567/230328208-f196b88e-3eee-4042-a33c-76da50d0e330.png">
