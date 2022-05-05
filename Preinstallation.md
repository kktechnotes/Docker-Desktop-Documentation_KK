# Preinstallation
This topic describes the prerequisites required to install Docker Desktop on Windows.
## System Requirements
Before installing the Docker Desktop application, your system must meet the following hardware and software requirements:
- **RAM**: 4GB or above
- **Processor**: 64-bit processor with [Second Level Address Translation (SLAT)](https://en.wikipedia.org/wiki/Second_Level_Address_Translation)
- **Operating System**
  - Windows 11 (64-bit): Home or Pro version 21H2 or higher, or Enterprise or Education version 21H2 or higher.
  - Windows 10 64-bit: Home or Pro 2004 (build 19041) or higher, or Enterprise or Education 1909 (build 18363) or higher.
- **Additional Configuration**: You must congifure the following components:
  - Enable Windows Subsystem for Linux Version 2 (WSL 2) in Windows
  - Enable Virtualization support at BIOS level
### Setup: Enable WSL 2 on Windows Operating System (OS)
This section explains steps to enable WSL 2 in Windows Operating System
> **Tip**: Before installation, you can perform the [steps to check](#check-wsl-2-on-your-system) if you already have WSL2 enabled on your system.

> **Before you Begin**: You must enable [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-1---enable-the-windows-subsystem-for-linux) and [Check requirements for running WSL 2](https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-2---check-requirements-for-running-wsl-2) .
1. Download the [Linix Kernel Update](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) package. The Windows Installer Package is downloaded. 
2. Double-click the package and follow the instructions.
3. Click **Finish**. The WSL 2 package is installed on the sytem.
4. Press the Windows key on your keyboard and type "Windows Powershell" in the search box
5. Type or copy/paste the following command
  ```
  wsl --set-default-version 2
  ```
**Result**: The message, "The operation is completed successfully," is displayed.

#### Check WSL 2 on your system
1. Press the Windows key on your keyboard
2. In the search box, type "Windows Powershell"
3. Type or copy/paste the following command
```
{
wsl --status
}
```
**Result**: If WSL 2 is enabled, then `Default Version: 2` is displayed.


