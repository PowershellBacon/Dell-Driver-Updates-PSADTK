# Dell-Driver-Updates-PSADTK
Dell Driver update w/ Powershell Application Deployment ToolKit. This package for SCCM will use Dell's Command Update command line to scan the computers for hardware, then cross check it with Dell's model catalog and install the drivers from Dell's site. This includes Bios and Drivers. 


Added switch for UpdateType (All, Bios, Network, Display)
  Default: All

Example: Deploy-Application.exe -UpdateType Bios  
  Result: Updates ONLY the bios on the workstation
  
Example: Deploy-Application.exe -UpdateType Network  
  Result: Updates ONLY the network driver(s) on the workstation, Wifi and/or Lan
  
Example: Deploy-Application.exe -UpdateType Display  
  Result: Updates ONLY the display drivers on the workstation
  
Example: Deploy-Application.exe  
  Result: Updates ALL the drivers on the workstation

Note: Make sure if you have a BIOS password on the system you update the PW in the script, if you do not employ a bios pw commment out the cctk lines of the code.
