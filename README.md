# Add Store to Windows 10 Enterprise LTSC  

For Windows 10 Enterprise LTSC 2019
[Download](https://github.com/lixuy/LTSC-Add-MicrosoftStore/archive/2019.zip)  

## To install, run Add-Store.cmd as Administrator  

If you do not want App Installer / Purchase App / Xbox identity, delete each one appxbundle before running to install. However, if you plan on installing games or any app with in-purchase options, you should include everything.  
If the store still will not function, reboot. If still not working, open the command prompt as the administrator and run the following command, then reboot once more.  

```PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"```

## Addition troubleshooting
>
>Right click start  
Select Run  
Type in: WSReset.exe  
This will clear the cache if needed.  
  
abbodi1406：
<https://forums.mydigitallife.net/threads/add-store-to-windows-10-enterprise-ltsc-LTSC.70741/page-30#post-1468779>
