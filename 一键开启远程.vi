@echo off
title 开3389小工具 
cls
rem 开启3389
reg add "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server" /v fDenyTSConnections /t REG_DWORD /d 00000000 /f >nul
echo.
echo 提示你：3389已经开启
echo.
rem 提取本机IP地址
for /f "tokens=15" %%a in ('ipconfig^|find "IP Address"') do set ip=%%a
echo 本机的IP是%ip%&ping 127.1 -n 5 >nul
exit
