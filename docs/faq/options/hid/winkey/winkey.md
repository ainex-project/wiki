<!--- This file is a snippet --->
The following settings all follow the same rules.

The value must be a key identifier, or multiple key identifiers separated by spaces.<br/>
Modifiers may be added to change the meaning of a bind when another key is pressed.

Key identifiers may be:
- [Virtual-Key Codes](https://docs.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes) (hex)
- A character corresponding to a key

Key modifiers are:

|**modifier**|**meaning**        |
|:-----------|:-----------------:|
|`_`         |only with Caps Lock|
|`^`         |only with Shift    |

Examples:

|**config value**            |**meaning**                                                         |
|:---------------------------|:------------------------------------------------------------------:|
|`keybind_a = "0xBA"`        |bind the :regional_indicator_a: button to the ; key                 |
|`keybind_x = "X"`           |bind the X button to the X key                                      |
|`keybind_y = "Y U 0xA0"`    |bind the Y button to the Y key, the X key and the Left Shift key.   |
|`keybind_b = "_0xBA"`       |bind the B button to the ; key only when Caps Lock is enabled       |
|`keybind_dpad_up = "^X"`    |bind the :down_arrow: button to the X key only when Shift is pressed|

|**setting_name**         |**default_value**|**meaning**                                          |
|:------------------------|:---------------:|:----------------------------------------------------|
|keybind_a                |0xBA             |Bind A to ;                                          |
|keybind_b                |0xDE             |Bind B to "                                          |
|keybind_back             |Z                |Bind Back to Z                                       |
|keybind_dpad_down        |^S               |Bind :arrow_down: to
|keybind_dpad_left        |^A               |
|keybind_dpad_right       |^D               |
|keybind_dpad_up          |^W               |
|keybind_left_shoulder    |1                |
|keybind_left_thumb       |F                |
|keybind_left_thumb_down  |_S               |
|keybind_left_thumb_left  |_A               |
|keybind_left_thumb_right |_D               |
|keybind_left_thumb_up    |_W               |
|keybind_left_trigger     |Q I              |
|keybind_right_shoulder   |3                |
|keybind_right_thumb      |K                |
|keybind_right_thumb_down |0x28             |
|keybind_right_thumb_left |0x25             |
|keybind_right_thumb_right|0x27             |
|keybind_right_thumb_up   |0x26             |
|keybind_right_trigger    |E O              |
|keybind_start            |X                |
|keybind_x                |L                |
|keybind_y                |P                |
