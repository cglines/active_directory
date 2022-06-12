# 01 Installing the Domain  Controller

1. Use `sconfig` to:
    - Change the Hostname
    - Change the IP Address to Static
    - Change the DNS server to our own IP address

2. Install the Active Directory Windows Feature

```shell 
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
```

```
Get-NetIPAddress
```


# Joining the Workstation to the Domain Controller



```
Add-Computer -Domainname jelly.com -Credential jelly/administrator -Force -Restart
```
