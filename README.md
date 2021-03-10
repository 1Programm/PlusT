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
|   S1  |  S2  |  S3  |  S4  |  S5  |  S6  |  S7   |
|--------------------------------------------------|
                         |
|--------------------------------------------------|
|  Framework (fw)  |                               |
|..................................................|
| Graphics | Input | Sound | Objects | Utils | ... |
|--------------------------------------------------|
```

| Name | Type | Module - Links |
|---|---|---|
| Engine | Core | [\[plust-engine-api\]](https://github.com/1Programm/PlusT/tree/master/plust-engine-api) [\[plust-engine-basic\]](https://github.com/1Programm/PlusT/tree/master/plust-engine-basic) [\[plust-engine-starter\]](https://github.com/1Programm/PlusT/tree/master/plust-engine-starter) |
| | | |
| MessageBus | Core | [\[plust-messagebus-api\]](https://github.com/1Programm/PlusT/tree/master/plust-messagebus-api) [\[plust-messagebus-basic\]](https://github.com/1Programm/PlusT/tree/master/plust-messagebus-basic)|
| | | |
| S1: Framework | Controller / Handler | [\[plust-fw-api\]](https://github.com/1Programm/PlusT/tree/master/plust-fw-api) [\[plust-fw-lwjgl\]](https://github.com/1Programm/PlusT/tree/master/plust-fw-lwjgl) [\[plust-fw-swing\]](https://github.com/1Programm/PlusT/tree/master/plust-fw-swing) |
| S2: Scene     | Controller / Handler | [\[plust-sys-scene-api\]](https://github.com/1Programm/PlusT/tree/master/plust-sys-scene-api) |
| S3: Objects   | Controller / Handler | [\[plust-sys-objects-api\]](https://github.com/1Programm/PlusT/tree/master/plust-sys-objects-api) |
| S4: Collision | Controller / Handler | [\[plust-sys-collision-api\]](https://github.com/1Programm/PlusT/tree/master/plust-sys-collision-api) |
| S5: Input     | Controller / Handler | [\[plust-sys-input-api\]](https://github.com/1Programm/PlusT/tree/master/plust-sys-input-api) |
| S6: Sound     | Controller / Handler | [\[plust-sys-sound-api\]](https://github.com/1Programm/PlusT/tree/master/plust-sys-sound-api) |
| S7: Animation | Controller / Handler | [\[plust-sys-animation-api\]](https://github.com/1Programm/PlusT/tree/master/plust-sys-animation-api) |

Systems:
========
### [\[S1\] Framework:](link/System-Framework)
Controller to to the MessageBus when to run lifecycle methods of the Framework

### [\[S2\] Scene:](link/System-Scene)
Handels a list of scenes and how to load and unload them.

### [\[S3\] Objects:](link/System-Objects)
Handels a list of objects which be different on each Scene.

### [\[S4\] Collision:](link/System-Collision)
Handels Collision between Objects. Will be called by the [\[S3\] Object - System](link/System-Objects). 

### [\[S5\] Input:](link/System-Input)
Manages Settings for which physical key binds to which In - Game - Controll Input.

### [\[S6\] Sound:](link/System-Sound)
Manages all sound flow. All Sound can be disabled, enabled or changed there. 

### [\[S7\] Animation:](link/System-Animation)
Handles running Animation States.
