# Guest Network Lib

## ABOUT

The script is created to enable / disable the guest network

The script contains functions:

 - getGuestInterfacesArray - return $guestInterfaces
 - checkGuestStatus - check status guest network ans set same by Led and Guest network
 - switchGuestStatus - switch Status Guest network and Led
 
The script needs libraries:

 - [`LED Lib`](https://github.com/nrgiver/MikroTikScripts/tree/master/LED%20Lib)
 
The script needs policies:

 - read
 - write
 
## Examples

Get Interfases Guest Network (ex. Other Script)

      :local guestInterfaces [[:parse [/system script get guest_lib source]] action=getGuestInterfacesArray];

Check and Set same status Guest network and Led (ex. Sheduler)

      [[:parse [/system script get guest_lib source]] action=checkGuestStatus];

Switch Status Guest Network (ex. Press Button)

      [[:parse [/system script get guest_lib source]] action=switchGuestStatus];

[`nrgiver/MikroTikScripts`](https://github.com/nrgiver/MikroTikScripts)