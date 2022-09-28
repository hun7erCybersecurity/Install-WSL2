[<img src='https://cdn.pixabay.com/photo/2011/08/14/18/08/penguin-8640__340.png' alt='LinuxLogo' height='120'>](https://github.com/hun7erCybersecurity)




# Install-WSL2
## Here you will find how you install WSL2 on a Windows operating system.

###  My Source

* [Lern Mircrosoft (Install Manual)](https://learn.microsoft.com/en-us/windows/wsl/install-manual)
* [Lern Mircrosoft (Basic Commands)](https://learn.microsoft.com/en-us/windows/wsl/basic-commands#install-a-specific-linux-distribution)
* [Freecodecamp](https://www.freecodecamp.org/news/how-to-install-wsl2-windows-subsystem-for-linux-2-on-windows-10/)



## Install WSL2 with Powershell:
* Enable Windows features for WSL 
* Check requirements for running WSL 2
* test
* test


## Enable Windows features for WSL:
1. Start your Powershell as Administrator.

<br />

2. Copy and Execute these commands line by line

```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux -All -NoRestart

Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform -All -NoRestart

Restart-Computer

```
<br />

3. After the reboot of your system, check with these commands if the state of the Optional features are Enabled

```
Get-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux | Select-Object State

Get-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform | Select-Object State
```

<br />

## Check requirements for running WSL 2

1. To update to WSL 2, you must be running Windows 10...

   * For x64 systems: Version 1903 or later, with Build 18362 or later.
   * For ARM64 systems: Version 2004 or later, with Build 19041 or later.
   
<br/>

2. Copy and execute this command to check your Version of the running Opertatingsystem

```   
[environment]::OSVersion.Version | Select-Object Build
```
# to be countinue....
