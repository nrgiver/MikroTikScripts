# Date Lib

## ABOUT

The script is created to create timestamps and store an array of months in one place

The script contains functions:

 - getMonthArray - return $guestInterfaces
 - getTimeStamp - get TimeStamp formated YYYYMMDD-hhmmss
 
The script needs policies:

 - read
 
## Examples

Get Array of Months in RouterOS (ex. Other Script)

      :local months [[:parse [/system script get date_lib source]] action=getMonthArray];

get TimeStamp formated YYYYMMDD-hhmmss (ex. Other Script)

      :local timestamp [[:parse [/system script get date_lib source]] action=getTimeStamp];

[`nrgiver/MikroTikScripts`](https://github.com/nrgiver/MikroTikScripts)