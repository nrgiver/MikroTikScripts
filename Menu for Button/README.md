# Menu for Press Button

## ABOUT

The script is created to be able to call different functions depending on the number of Press Button
 
The script needs libraries:

 - [`Backup Lib`](https://github.com/nrgiver/MikroTikScripts/tree/master/Backup%20Lib)
 - [`Guest Lib`](https://github.com/nrgiver/MikroTikScripts/tree/master/Guest%20Lib)
 - [`LED Lib`](https://github.com/nrgiver/MikroTikScripts/tree/master/LED%20Lib)
 
The script needs policies:

 - ftp
 - read
 - write
 - for backup: policy, test
 
## Examples

This is just script - just run it or write to it in the Press Button event:

      /system routerboard mode-button set enabled=yes on-event=button_menu

[`nrgiver/MikroTikScripts`](https://github.com/nrgiver/MikroTikScripts)