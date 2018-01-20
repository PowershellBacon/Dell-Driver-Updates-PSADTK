# Dell-Driver-Updates-PSADTK
Dell Driver update w/ Powershell Application Deployment ToolKit

This now wrapped in the Powershell App Deployment Toolkit

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
