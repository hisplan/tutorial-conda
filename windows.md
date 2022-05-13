# Windows

## Install WSL

For Windows users, it's much better to use Windows Subsystem for Linux (WSL).

To install WSL, you must be running Windows 10 version 2004 and higher (Build 19041 and higher) or Windows 11.

To check your Windows version and build number, press `Windows logo key + R`, type `winver`.

Press `Windows logo key`, type `cmd`, select `Run as administrator` to open a new terminal window. Run the following command to install WSL:

```
wsl --install
```

Once you have successfully installed WSL, skip to the `Set Up WSL` section.

If the above command returns an error message, something like `wsl is not a recognized command`, then follow the instructions below.

Press `Windows logo key`, type `cmd`, select `Run as administrator` to open a new terminal window.

Run the following command:

```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

Run the following command:

```
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

Restart your machine.

Press `Windows logo key`, type `cmd`, select `Run as administrator` to open a new terminal window.

Run the following command:

```
wsl --install
```

## Set Up WSL

Once you have successfully installed WSL, restart your machine. You will be prompted to create a user account and password for your newly installed Linux distribution.

Run the following commands to install the latest Ubuntu updates:

```
sudo apt-get update -y
sudo apt-get upgrade -y
```

## Install Windows Terminal

WSL gives you Ubuntu terminal by default, but **Windows Terminal** from the Microsoft Store is recommended because it allows you to have multiple terminals in the same window.
