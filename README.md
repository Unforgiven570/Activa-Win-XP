# Activa-Win-XP
# Archivo por lotes para activar Windows XP

#Inicio de activador


taskkill /im wgatray.exe 
Del c:\Windows\System32\WgaTray.exe 
Del c:\Windows\System32\dllcache\WgaTray.exe 
echo Windows Registry Editor Version 5.00 >%temp%\WGANFIX.REG 
echo. >>%temp%\WGANFIX.REG 
echo [-HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\Notify\WgaLogon] >>%temp%\WGANFIX.REG 
regedit /s %temp%\WGANFIX.REG 
del %temp%\WGANFIX.REG 
del c:windows\system32\wgalogon.dll 
del c:windows\system32\dllcache\wgalogon.dll 


#Fin de Avtivador
