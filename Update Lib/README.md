# Update Lib

## ABOUT

The script is created to automate the update of Router Board and RouterOS

The script contains functions:

 - updateRouterBoard - Check new version RouterBoard and if it exists then Create Backup and Update
 - updateRouterOS - Check new version RouterOS and if it exists then Create Backup and Update
 
The script needs libraries:

 - [`Backup Lib`](https://github.com/nrgiver/MikroTikScripts/tree/master/Backup%20Lib)
 
The script needs policies:

 - ftp
 - read
 - write
 - for backup: policy, test
 
## Examples

Check new version RouterBoard and if it exists then Create Backup and Update (ex. Sheduler)

      [[:parse [/system script get update_lib source]] action=updateRouterBoard];

Check new version RouterOS and if it exists then Create Backup and Update (ex. Sheduler)

      [[:parse [/system script get update_lib source]] action=updateRouterOS];

[`nrgiver/MikroTikScripts`](https://github.com/nrgiver/MikroTikScripts)