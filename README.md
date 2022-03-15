![ReleaseVersion](https://img.shields.io/github/v/release/mr4lexndr/HomeBoard)
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].


[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

# HomeBoard
Simple ESP32 based 4 Channel LV board for controlling Home appliances with [HomeSpan](https://github.com/HomeSpan/HomeSpan).
HomeBoard was created to controll variety of LED strips, and other Low voltage appliances. 

![HomeBoard](https://github.com/mr4lexndr/HomeBoard/blob/main/Images/HomeBoard_transparent.png)

## Main Features
- Supply Voltage 4-30V
- Status LED and Control push button for easy configuration
- 4 PWM-eabled channels (0-Vin V, 25A)
- 2 channels can be configured with Logic Level Shifters to drive Neopixels etc.
- Switch or button option vailable.


## User Integration with HomeSpan
Status LED and Control Button are attached to deafault pins for most of the boards. S1 Button is used as boot button as well during programming
- LED - GPIO2
- Button - GPIO0

## Variants
Four channels can be configured per requiremnts. Specific sections 1-3 has been marked on PCB. Only one group from each section should be soldered based on selected funtion. Available options:

| Channel | Main Function | Alternative |
| ------- | ------------- | ----------- |
| 1       | Open Drain    | Logic Level (0-Vin) |
| 2       | Open Drain    | Logic Level (0-Vin) |
| 3       | Open Drain    | Switch (GPIO18)     |
| 4       | Open Drain    | Switch (GND)        |

