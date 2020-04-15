# Menu for Press Button

## ABOUT

The script is designed to automate the creation of backups

The script allows you to configure the cleaning of old backups

The script supports saving backups to the USB drive

The script contains functions:

 - getBackupsPath - Return $backupsPath
 - createBackup - Create backup and export with mark about your $reason
 - clearOldBackup - Clear old backup over then $overMonths months
 
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