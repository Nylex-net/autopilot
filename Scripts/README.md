# Running Scripts

## Get-WindowsAutoPilotInfo.ps1

_Disclaimer_: The PowerShell script _Get-WindowsAutoPilotInfo.ps1_ is not mine. It was made by Microsoft, and can be installed using the instructions below.

Open PowerShell as administrator and install the script using the following command:

`Install-Script -Name Get-WindowsAutopilotInfo`

### Generate your own CSV file

Run `Get-WindowsAutopilotInfo.ps1 –OutputFile D:\\Devices\\Device1.csv` as administrator in PowerShell.  Be sure to replace the `D:\\Devices\\Device1.csv` with your desired path.

### Import a device hash directly into Intune

Run `Get-WindowsAutoPilotInfo.ps1 -online -GroupTag "Autopilot-Devices" -Assign` as administrator in PowerShell.  Replace the tag name to your desired name.
