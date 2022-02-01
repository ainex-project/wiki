<!--- This file is a snippet --->
The following settings all follow the same rules.

The value must be a key identifier, or multiple key identifiers separated by spaces.<br/>
Modifiers may be added to change the meaning of a bind when another key is pressed.

## Key identifiers
- [Virtual-Key Codes](https://docs.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes) (hex)
- A character corresponding to a key

Key modifiers are:

|**modifier**|**meaning**        |
|:-----------|:-----------------:|
|`_`         |only with Caps Lock|
|`^`         |only with Shift    |

## Examples

|**config value**            |**meaning**                                                         |
|:---------------------------|:------------------------------------------------------------------:|
|`keybind_a = "0xBA"`        |bind the :regional_indicator_a: button to the ; key                 |
|`keybind_x = "X"`           |bind the X button to the X key                                      |
|`keybind_y = "Y U 0xA0"`    |bind the Y button to the Y key, the X key and the Left Shift key.   |
|`keybind_b = "_0xBA"`       |bind the B button to the ; key only when Caps Lock is enabled       |
|`keybind_dpad_up = "^X"`    |bind the :down_arrow: button to the X key only when Shift is pressed|

## Default bindings

|**setting_name**         |**default_value**|**meaning**                                                   |
|:------------------------|:---------------:|:------------------------------------------------------------:|
|keybind_a                |0xBA             |Bind :xbox-a_button:A to ++semicolon++                        |
|keybind_b                |0xDE             |Bind :xbox-b_button:B to ++dblquote++                         |
|keybind_back             |Z                |Bind :xbox-back_button:Back to ++z++                          |
|keybind_dpad_down        |^S               |Bind :xbox-dpad_down:D-Pad Down to ++s++ (Caps Lock on)       |
|keybind_dpad_left        |^A               |Bind :xbox-dpad_left:D-Pad Left to ++a++ (Caps Lock on)       |
|keybind_dpad_right       |^D               |Bind :xbox-dpad_right:D-Pad Right to ++d++ (Caps Lock on)     |
|keybind_dpad_up          |^W               |Bind :xbox-dpad_up:D-Pad Up to ++w++ (Caps Lock on)           |
|keybind_left_shoulder    |1                |Bind :xbox-left_shoulder:Left Shoulder to ++1++               |
|keybind_left_thumb       |F                |Bind :xbox-left_stick_click:Left Stick Click to ++f++         |
|keybind_left_thumb_down  |_S               |Bind :xbox-left_stick_down:Left Stick Down to ++shift+s++     |
|keybind_left_thumb_left  |_A               |Bind :xbox-left_stick_left:Left Stick Left to ++shift+a++     |
|keybind_left_thumb_right |_D               |Bind :xbox-left_stick_right:Left Stick Right to ++shift+d++   |
|keybind_left_thumb_up    |_W               |Bind :xbox-left_stick_up:Left Stick Up to ++shift+w++         |
|keybind_left_trigger     |Q I              |Bind :xbox-left_trigger:Left Trigger to ++q++ and ++i++       |
|keybind_right_shoulder   |3                |Bind :xbox-right_shoulder:Right Shoulder to ++3++             |
|keybind_right_thumb      |K                |Bind :xbox-right_stick_click:Right Stick Click to ++k++       |
|keybind_right_thumb_down |0x28             |Bind :xbox-right_stick_down:Right Stick Down to ++up++        |
|keybind_right_thumb_left |0x25             |Bind :xbox-right_stick_left:Right Stick Left to ++left++      |
|keybind_right_thumb_right|0x27             |Bind :xbox-right_stick_right:Right Stick Right to ++right++   |
|keybind_right_thumb_up   |0x26             |Bind :xbox-right_stick_up:Right Stick Up to ++up++            |
|keybind_right_trigger    |E O              |Bind :xbox-right_trigger:Right Trigger to ++e++ or ++o++      |
|keybind_start            |X                |Bind :xbox-start_button:Start to ++x++                        |
|keybind_x                |L                |Bind :xbox-x_button:X to ++l++                                |
|keybind_y                |P                |Bind :xbox-y_button:Y to ++p++                                |
