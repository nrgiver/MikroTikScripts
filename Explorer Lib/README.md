# Explorer Lib

## ABOUT

Script created to create folders

The script uses the method of creating folders through SMB

The script contains functions:

 - makeDir - Check and create dir by SMB mythod
 
The script needs policies:

 - ftp
 - read
 - write
 
## Examples

Check exist and create dirs by path (ex. Other Script)

      [[:parse [/system script get explorer_lib source]] action=makeDir path="flash/dir/subdir/"];

[`nrgiver/MikroTikScripts`](https://github.com/nrgiver/MikroTikScripts)