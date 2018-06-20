# -API-to-navigate-a-rover-in-a-grid
Build an API to navigate a rover along a topographical grid representation of Mars.

Requirements  
  - The rover when initialized will have an initial starting point (x, y) as well as a direction (N, S, E, W) that it is facing.
  - The rover should recieve its commands as a string array. It should then iterate over the array executing the commands in sequence until either a) all commands have succeeded in which case return a OK status along with location and direction or b) a command failed due to an obstacle in which case return an OBSTACLE status code along with last successful location and direction
  - If the rover recieves invalid commands immediatly an INVALID_COMMAND status along with location and direction of the last successful command
  - The rover may move forward/backward with the (F, B) commands
  - The rover may turn left and right with the (L, R) commands
  - If the rover encounters obstacles in the terrain then it should return its last successfull location as well as a OBSTACLE status
  - If the rover encounters the edge of the world it should stop and return its last successfull location as well as a OBSTACLE status
  
  The [JSFiddle](https://jsfiddle.net/shiva21/xnwfxxz4/14/) has the implementation of the solution for the problem.
