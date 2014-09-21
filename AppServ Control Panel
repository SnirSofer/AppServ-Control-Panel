@echo off
title AppServ Control Panel - By s4f3
color b
:menu
echo 1 - Turn Off Apache
echo 2 - Turn On Apache
echo 3 - Restart Apache
echo 4 - Turn Off MySQL
echo 5 - Turn On MySQL
echo Please choose one of the options

set /p choice=[Method id]: 
if "%choice%" == "1" goto :apacheoff
if "%choice%" == "2" goto :apacheon
if "%choice%" == "3" goto :apacherst
if "%choice%" == "4" goto :sqloff
if "%choice%" == "5" goto :sqlon
if "%choice%" == "clear" cls
goto :menu

:apacheoff
cls
cd C:\AppServ\Apache2.2\bin\
echo Please wait to stop Apache...
httpd.exe -k stop -n Apache2.2
goto :menu

:apacheon
cls
echo Please wait to start Apache...
cd C:\AppServ\Apache2.2\bin\
httpd.exe -k start -n Apache2.2
goto :menu

:apacherst
cls
echo Please wait to restart Apache...
cd C:\AppServ\Apache2.2\bin\
httpd.exe -k restart -n Apache2.2
goto :menu

:sqloff
cls
echo Please wait to stop MySQL...
cd C:\AppServ\MySQL\
net stop MySQL
echo #######  Stopping MySQL Service  #######
goto :menu

:sqlon
cls
echo Please wait to start MySQL...
cd C:\AppServ\MySQL\
net start MySQL
echo #######  Starting MySQL Service  #######
goto :menu



:quit
echo Bye Bye Owner!
pause
