Moving marker.js - A file which **must** be there for the animation to take place (L.Routing is dependent on this file)

sim.html - In this, one marker is placed on the map based on its lattitude and longitude coordinates entered in the code. The other marker can be selected on our own by clicking another point in the map. The initial marker then sets a route to the place which we have selected and animates itself to the selected final marker.

coordinates.html - The lattitude and the longitude of the marker on the map are displayed as the output. The coordinates of a place can be obtained by clicking on it.

index.html - Assuming there are 2 markers (the initial destination and the final destionation. However the code contains 6 markers, which is 3 trips in total). When the initial marker is clicked, a bouncing animation takes place and then animates itself to the final destionation via a route which is found by the L.Routing function. However, if there are multiple trips, 
**the markers which indicate the initial points of the respective trips must be clicked sequentially** in the order in which they have been written in the code (the second trip cannot start unless the first trip starts).
