# CertConverter-Context-Entry-Windows
WIP. Context menu entry to convert a .pem certificate into other formats.


- Enable Subsystem:
`Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

- Prompt to reboot, if subsystem got enabled for the first time
https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/restart-computer?view=powershell-7.2
`Restart-Computer -Confirm`


Base64-encoded or DER-encoded binary X.509 Certificate
```shell
openssl x509 -outform der -in RSA-chain.pem -out rsa-chain.crt
openssl x509 -outform der -in RSA-cert.pem -out rsa-cert.crt
```


```shell
openssl x509 -outform der -in RSA-cert.pem -out rsa-cert.key
```
