# DirectCurrent Motor Module

[![](https://img.shields.io/badge/Available_in_the_Arduino_Library_Manager-2ea44f)](https://www.arduino.cc/reference/en/libraries/engine-control/)

## Get Started

**Import**

1. Look up `DirectCurrent-Motor-Module` in the Library Manager and install the latest version
2. Insert the following snippet
 
```ino
#include <DirectCurrent-Motor-Module.h>
```

**Setup**

```ino
DirectCurrent [name] = { int input1, int input2, int dc };
```
**Parameters**

* `[name]` Use a name without spaces
* `input1` IN1 Pin
* `input2` IN2 Pin
* `dc` DC Pin

**Example**

```ino
DirectCurrent example = { 1, 2, 3 };
```

**Use**

```ino
moveDirectCurrent(DirectCurrent i, int mode1, int mode2, int speed);
```

**Description** Move the DC motor

**Parameters**
* `i` Name defined in the setup
* `mode1` Enable or disable the `input1` pin with `0` (disable) and `1` (enable)
* `mode2` Enable or disable the `input2` pin with `0` (disable) and `1` (enable)
* `speed` Motor speed `Max. Value` 255

**Example**

```ino
moveDirectCurrent(example, 1, 202);
```
