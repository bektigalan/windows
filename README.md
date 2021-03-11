# windows


how to fix windows 10 activation
error code
0xc0ea000a

1. sync time to internet time
2. open windows powershell and paste this
```
Get-AppxPackage -allusers Microsoft.WindowsStore | Foreach
{Add-AppxPackage -DisableDevelopmentMode -Register
“$($_.InstallLocation)\AppXManifest.xml”}
```
3. open cmd as admin, and type ```wsreset.exe``` and hit enter