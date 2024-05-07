<!--- This file is a snippet --->
Disable real-time clock scaling code.<br/>
Time management and locking is bypassed.
Guest system time is directly pulled from the host.

| **clock_no_scaling**                                                    | **bool** |
|:------------------------------------------------------------------------|:--------:|
| Guest time is scaled proportionally to the running speed. (**default**) |  false   |
| System time is pulled from directly the host.                           |   true   |
