# checkPing
Check your ping to various League of Legends Server
Copy the below code
Open a text editor like notepad(NOT word or wordpad)
Save this as batchfile.bat, make sure there is no .txt extension after the .bat

@echo off & cls

color 0C
ECHO *********************
ECHO * LoL ping checker  *
ECHO *  oo Kylo Ren oo   *
ECHO *********************

:Start
ECHO.
ECHO 	[1] EUW
ECHO 	[2] EUNE
ECHO 	[3] NORTH AMERICA
ECHO 	[4] RUSSIA
ECHO 	[5] BRAZIL
ECHO 	[6] JAPAN
ECHO 	[7] LATIN AMERICA 1
ECHO 	[8] LATIN AMERICA 2
ECHO 	[9] OCEANIC
ECHO 	[0] TURKEY
ECHO 	[X] EXIT
ECHO.

set /p a=
IF %a%==1 GOTO checkEUW
IF %a%==2 GOTO checkEUNE
IF %a%==3 GOTO checkNA
IF %a%==4 GOTO checkRU
IF %a%==5 GOTO checkBR
IF %a%==6 GOTO checkJP
IF %a%==7 GOTO checkLA1
IF %a%==8 GOTO checkLA2
IF %a%==9 GOTO checkOC
IF %a%==0 GOTO checkTR
IF %a%==x GOTO END

:checkEUW
ECHO *********************************
ECHO * CHECKING PING FOR EUROPE WEST *
ECHO *********************************
ping 185.40.64.65
ECHO ********
ECHO * DONE *
ECHO ********
GOTO Start

:checkEUNE
ECHO *******************************
ECHO * CHECKING PING FOR EUROPE NE *
ECHO *******************************
ping 64.7.194.1
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkNA
ECHO ***********************************
ECHO * CHECKING PING FOR NORTH AMERICA *
ECHO ***********************************
ping 192.64.174.65
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkRU
ECHO ****************************
ECHO * CHECKING PING FOR RUSSIA *
ECHO ****************************
ping 185.40.64.99
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkBR
ECHO ****************************
ECHO * CHECKING PING FOR BRAZIL *
ECHO ****************************
ping 66.151.33.20
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkJP
ECHO ***************************
ECHO * CHECKING PING FOR JAPAN *
ECHO ***************************
ping 104.160.154.194
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkLA1
ECHO *************************************
ECHO * CHECKING PING FOR LATIN AMERICA I *
ECHO *************************************
ping 66.151.33.24
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkLA2
ECHO **************************************
ECHO * CHECKING PING FOR LATIN AMERICA II *
ECHO **************************************
ping 66.151.33.28
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkOC
ECHO *****************************
ECHO * CHECKING PING FOR OCEANIC *
ECHO *****************************
ping 192.64.169.20
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:checkTR
ECHO ****************************
ECHO * CHECKING PING FOR TURKEY *
ECHO ****************************
ping 185.40.64.105
ECHO ********
ECHO * DONE *
ECHO ******** 
GOTO Start

:END
