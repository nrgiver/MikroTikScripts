# LED Lib

## ABOUT

The script is designed to control LEDs

The script contains functions:

 - switchDarkMode - Switch Dark Mode
 - setStatusLed - Check and set the status Led
 - blinkLed - Blink Led $count times

The script needs policies:

 - read
 - write
 
## Examples

On Led (ex. Other Script)

      [[:parse [/system script get led_lib source]] action=setStatusLed status=on];

Blink Led 5 times (ex. Other Script)

      [[:parse [/system script get led_lib source]] action=blinkLed count=5];

Switch Dark Mode (ex. Press Button)

      [[:parse [/system script get led_lib source]] action=switchDarkMode];

[`nrgiver/MikroTikScripts`](https://github.com/nrgiver/MikroTikScripts)