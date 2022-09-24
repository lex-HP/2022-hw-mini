# Hardware miniproject
* Alex Hureaux-Perron (alexchp@bu.edu)
* Wenyu (Jessica) Hu (wjhu@bu.edu)

This project consists of making a Pico microcontroller's LED blink. In order to make it work, the computer runs Windows Subsystem for Linux (WSL). In WSL, the cloned github repository requires cmake for compilling. The C code "[pmw_led_fade_original.c](https://github.com/lex-HP/2022-hw-mini/blob/main/src/pwm/led_fade/pwm_led_fade_original.c)" is the untouched version that makes the LED blink in a standard manner and "[pwm_led_fade.c](https://github.com/lex-HP/2022-hw-mini/blob/main/src/pwm/led_fade/pwm_led_fade.c)" is the altered version.  The altered version increases the dimming speed of the Pico LED thanks to the following changed line 

```sh
fade--;
```
became 
```sh
fade = fade - 50;
```
Therefore the LED decreases 50 times faster 

The original and altered version are running side by side in this video ([Miniproject.mp4](https://github.com/lex-HP/2022-hw-mini/blob/main/Miniproject.mp4))
