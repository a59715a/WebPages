"# WebPages" 

https://a59715a.github.io/WebPages/direct.html?url=LTCexe:c:\\tch\\exe\\ClickOnceOpen.exe

.reg
Windows Registry Editor Version 5.00 
[HKEY_CLASSES_ROOT\LTCexe] 
@="URL:Your App Protocol" 
"URL Protocol"="" 
[HKEY_CLASSES_ROOT\LTCexe\DefaultIcon] 
@="\"ClickOnceOpen.exe\",1" 
[HKEY_CLASSES_ROOT\LTCexe\shell] 
[HKEY_CLASSES_ROOT\LTCexe\shell\open] 
[HKEY_CLASSES_ROOT\LTCexe\shell\open\command] 
@="\"C:\\TCH\\exe\\ClickOnceOpen.exe\" \"parameter=%1\"" 
[HKEY_CLASSES_ROOT\iehttp] 
@="URL:Open with IE Protocol" 
"URL Protocol"="" 
[HKEY_CLASSES_ROOT\iehttp\shell] 
[HKEY_CLASSES_ROOT\iehttp\shell\open] 
[HKEY_CLASSES_ROOT\iehttp\shell\open\command] 
@="cmd /V /C \"set URL=%1&& set URL=!URL:iehttp=http!&&cmd /c \"\"C:\\Program Files (x86)\\Internet Explorer\\iexplore.exe\"\" !URL!\"" 
[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome] 
"AutoLaunchProtocolsFromOrigins"="[{\"protocol\": \"iehttp\",\"allowed_origins\": [\"*\"]}]" 


.bat
copy \\HISSVR\TCHEXE$\EXE\ClickOnceOpen.exe c:\tch\exe\ClickOnceOpen.exe
