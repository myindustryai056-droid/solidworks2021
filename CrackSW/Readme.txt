00. Before installation, block the outgoing Internet access by means of Windows 
   Firewall or cord plug. Check .NET Framework 3.5 and 4.0 are installed. If
   .NET Framework 3.5 (including 2.0) is not installed, go to 
   "Control Panel" -> "Programs and Features" -> "Turn Windows features on or off" ->
   -> select ".NET Framework 3.5 (including 2.0)"

000. Uninstall (if exist) SolidWorks_Flexnet_Server from previuos SSQ's releases!
    To do it run as Administrator SolidWorks_Flexnet_Server\server_remove.bat 
    and wait until service "SolidWorks Flexnet Server" will be removed
    After that delete SolidWorks_Flexnet_Server folder from computer 

1. Run "sw2024_network_serials_licensing.reg" and confirm to add info 
   into Windows Registry

2. Copy folder "SolidWorks_Flexnet_Server" to C: , run as Administrator
   "SolidWorks_Flexnet_Server\server_install.bat" and wait until new service 
   "SolidWorks Flexnet Server" will be install and started

3. Run SolidWorks 2024 setup
   If select to "Install server components" > SOLIDWORKS PDM Server- do not install 
   SolidNetwork License Manager!
   When asked of License Server definition input: 25734@localhost

   3.1 If the System Check Warning window appears, ignore it (click Next to continue)

   3.2 If the warning "SolidWorks Serial number was not found in activation database" 
       appears, ignore it (click OK to continue)

   3.3 If the full list of SW products to install is not visible,
       click "Select different package" and tick option 
       "Select products not included in this package"

   3.4 Select SW products to be installed

   3.5 If the "The Installation Manager was unable to determine the current subscription 
       expiration date. Would you like to reactivate your license to update this information?"
       appears, press No and press Yes in "Do you want to do it later?" prompt.

4. After end of setup 
   
   4.1 Run Windows Task Manager > Details
       Find (if exist) process "sldworks_fs.exe" > right mouse click > remove the task

   4.2 Delete (if exist) file C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS\netapi32.dll

   4.3 Remane (if exist) file C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS PDM\StoredProcs.dll
       to StoredProcs.dll.bak

   4.4. Copy folders from crack folder "SOLIDWORKS Corp" on top of original ones in folder
        C:\Program Files\SOLIDWORKS Corp\ (if folders with the same names exist)

5. Run "SolidSQUADLoaderEnabler.reg" and confirm to add info 
   into Windows Registry

6. REBOOT COMPUTER!

7. Run SolidWorks > Help > SolidNetWork License Manager > License Order

   Use the "Move Up" and "Move Down" buttons to position Premium products with 
   the same name higher than Professional and Standard products

   Click "Apply" to save the settings

   Click "OK" to close the SolidNetWork License Manager

8. Enjoy

================