# Hardware miniproject
* Alex Hureaux-Perron (alexchp@bu.edu)
* Wenyu (Jessica) Hu (wjhu@bu.edu)

This project consists of making a Rasberry Pi Pico microcontroller's LED blink. In order to make it work on a computer with the Windows system, Windows Subsystem for Linux (WSL) was used. In WSL, the cloned github repository requires cmake for compilling. The C code "[pmw_led_fade_original.c](https://github.com/lex-HP/2022-hw-mini/blob/main/src/pwm/led_fade/pwm_led_fade_original.c)" is the untouched version that makes the LED blink in a standard manner and "[pwm_led_fade.c](https://github.com/lex-HP/2022-hw-mini/blob/main/src/pwm/led_fade/pwm_led_fade.c)" is the altered version.  The altered version increases the dimming speed of the Pico LED from the following change on line 40:

```sh
fade--;
```
became 
```sh
fade = fade - 50;
```
Therefore the LED dims 50 times faster. Which to the human eye, seems to gradually light up and suddenly switch off.

The original and altered version are running side by side in this video: [MiniProject.mp4](https://github.com/lex-HP/2022-hw-mini/blob/main/MiniProject.mp4)
