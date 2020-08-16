### Working with the Windows Subsystem Linux: A Cheat Sheet
Notes for Windows Subsystem Linux and using different Linux distros.

### Table of Contents:
---
- [Accessing Windows Files](#accessing-windows-files)
- [Sources](#sources)


### Accessing Windows Files from the Linux Terminal:
---

list all drives:

`ls -al /mnt  `

navigate to file in C drive:

`cd /mnt/c/myfile.txt       `

open a file in C drive:

`cat /mnt/c/myfile.txt       `

navigate to a specific user and their files:

`cd /mnt/c/Users/cd "name_of_user"`

* reccomended: keep a copy of your files in the Linux system for faster access. I usually accept the slugishness when I have my repo in my Documents.

### HTTP Request Magic:
---
- under construction.

### Upgrading to WSL2:

1. enable the Virtual Machine Platform on Powershell (Admin) with :
`dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart` and restart the computer.
2. Open Powershell (Admin) and `wsl --set-default-version 2`
3. If ` WSL 2 requires an update to its kernel component. For information please visit https://aka.ms/wsl2kernel` then visit the link and install the appropriate MSI. Them, run `wsl --set-default-version 2` again.

* [WSL Doc on Upgrading](https://docs.microsoft.com/en-us/windows/wsl/install-win10#update-to-wsl-2)

### Sources:
---
1. https://blogs.windows.com/windowsdeveloper/2016/07/22/fun-with-the-windows-subsystem-for-linux/
2. https://docs.microsoft.com/en-us/windows/wsl/install-win10
3. https://gto76.github.io/linux-cheatsheet/

### Misc:
An ode to WSL and its help boosting my productive output:
``` html

you make me
a better web developer,
an innovation that I got for free

A dual boot was the answer
before, windows files
available only to a necromancer.

now I hold several distros
I'm at the Linux disco
```
