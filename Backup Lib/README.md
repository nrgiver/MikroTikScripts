# Backup and Cleaner Lib

## ABOUT

The script is created to automate the creation of backups

The script allows you to configure the cleaning of old backups

The script supports saving backups to the USB drive

The script contains functions:

 - getBackupsPath - Return $backupsPath
 - createBackup - Create backup and export with mark about your $reason
 - clearOldBackup - Clear old backup over then $overMonths months
 
The script needs libraries:

 - [`Date Lib`](https://github.com/nrgiver/MikroTikScripts/tree/master/Date%20Lib)
 - [`Explorer Lib`](https://github.com/nrgiver/MikroTikScripts/tree/master/Explorer%20Lib)
 
The script needs policies:

 - ftp
 - read
 - write
 - policy
 - test
 
## Examples

Get Backups Path (ex. Other Script)

      :local backupsPath [[:parse [/system script get backup_lib source]] action=getBackupsPath];

Create backup and export with mark about your reason (ex. Sheduler)

      [[:parse [/system script get backup_lib source]] action=createBackup reason="auto_every_weak"];

Clear old backups over then 2 months (only backups younger than 2 months will be saved) (ex. Sheduler)

      [[:parse [/system script get backup_lib source]] action=clearOldBackup overMonths=2];

[`nrgiver/MikroTikScripts`](https://github.com/nrgiver/MikroTikScripts)