# RegShot CLI
This is literally just an addition to the command line RegShot from https://sourceforge.net/p/regshot/code/322/
In that version there is a RegShot_CMD.exe that can do comparison shots only.
This version allows you to take the shots as well.

## Notes:
- You cannot change where the output of the comparison goes. (I mean, unless you want to add that functionality yourself. I made this as a quick and dirty fix for myself) The final output will always be a text file starting with "~" in System32

- You cannot change what it will scan. It will always do a full recursive directory scan of the C:\ drive and of the registry. (Again, unless you want to fix that yourself.)

- You need to make sure your first shot file has the extension ".hivu"

- I only made one for ANSI not unicode

## Usage
Taking a RegShot:
```
Regshot_cmd-x(86 or 64)-ANSI.exe <Path to Store HIVU file>.hivu

EX:
---
Regshot_cmd-x64-ANSI.exe C:\Temp\Output.hivu
```


Comparing to a RegShot:
```
Regshot_cmd-x(86 or 64)-ANSI.exe <Path to Stored HIVU file>.hivu -C

EX: (Final output will be a text file in System32 starting with "~")
---
Regshot_cmd-x64-ANSI.exe C:\Temp\Output.hivu -C
```
