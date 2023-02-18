# asansor
+---------------+
|   Simulator   |
+---------------+
| - clock       |
| - event queue |
+---------------+
| + start()     |
| + stop()      |
+---------------+

+--------------+
|   Elevator   |
+--------------+
| - id          |
| - currentFloor|
| - destination |
| - direction   |
| - doorStatus  |
| - passengers  |
| - capacity    |
+--------------+
| + openDoor()  |
| + closeDoor() |
| + move()      |
| + addPassenger()|
| + removePassenger()|
| + getPassengerCount()|
| + isFull()    |
| + isIdle()    |
+--------------+

+-----------------+
|   ElevatorBank  |
+-----------------+
| - elevators     |
| - callButtons   |
| - floorButtons  |
+-----------------+
| + requestElevator()|
| + getCallButtons()|
| + getFloorButtons()|
+-----------------+

+-----------------+
|   CallButton    |
+-----------------+
| - floor         |
| - direction     |
| - pressed       |
+-----------------+
| + press()       |
| + reset()       |
| + isPressed()   |
| + getDirection()|
+-----------------+

+-----------------+
|   FloorButton   |
+-----------------+
| - floor         |
| - pressed       |
+-----------------+
| + press()       |
| + reset()       |
| + isPressed()   |
+-----------------+

+---------------+
|   Passenger   |
+---------------+
| - id          |
| - currentFloor|
| - destination |
| - arrived     |
+---------------+
| + arrived()   |
| + boardElevator()|
| + exitElevator()|
| + isArrived() |
+---------------+
