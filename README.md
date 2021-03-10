Plus 2.0 - 2D Game Engine

Structure:
==========

```
----------------------------------------------------
|                      Engine                      |
|--------------------------------------------------|
                         |
|--------------------------------------------------|
|                   Message Bus                    |
|--------------------------------------------------|
    |      |      |      |      |      |      |
|--------------------------------------------------|
|   S1  |  S2  |  S3  |  S4  |  S5  |  S6  |  S7   |  (Systems *1)
|--------------------------------------------------|
                         |
|--------------------------------------------------|
|  Framework (fw)  |                               |
|..................................................|
| Graphics | Input | Sound | Objects | Utils | ... |
|--------------------------------------------------|

*1:
  S1: Framework  -  Controller / Handler
  S2: Scene      -  Controller / Handler
  S3: Object     -  Controller / Handler
  S4: Collision  -  Controller / Handler
  S5: Input      -  Controller / Handler
  S6: Sound      -  Controller / Handler
  S7: Animation  -  Controller / Handler
```

Systems:
========
### [\[S1\] Framework:](link/System-Framework)
Controller to to the MessageBus when to run lifecycle methods of the Framework

### [\[S2\] Scene:](link/System-Scene)
Handels a list of scenes and how to load and unload them.

### [\[S3\] Object:](link/System-Object)
Handels a list of objects which be different on each Scene.

### [\[S4\] Collision:](link/System-Collision)
Handels Collision between Objects. Will be called by the [\[S3\] Object - System](link). 

### [\[S5\] Input:](link/System-Input)
Manages Settings for which physical key binds to which In - Game - Controll Input.

### [\[S6\] Sound:](link/System-Sound)
Manages all sound flow. All Sound can be disabled, enabled or changed there. 

### [\[S7\] Animation:](link/System-Animation)
Handles running Animation States.
