#Hardware miniproject
* Alex Hureaux-Perron (alexchp@bu.edu)
* Wenyu (Jessica) Hu (wjhu@bu.edu)

Using the original led_fade code, we increased the dimming speed of the Pico LED, the line
```sh
fade--;
```
became 
```sh
fade=fade-50;
```
