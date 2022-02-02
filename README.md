# CertConverter-Context-Entry-Windows
WIP. Context menu entry to convert a .pem certificate into other formats.


- Enable Subsystem:
`Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

- Prompt to reboot, if subsystem got enabled for the first time
https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/restart-computer?view=powershell-7.2
`Restart-Computer -Confirm`
