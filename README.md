# wsl-setup


1. Open Powershell from the search bar. You must right click and say run as administrator. 
2. Type wsl --install and then press enter.
3. You should see WSL and the Ubuntu being downloaded and installed.
4. Restart computer.
5. Open Powershell as administrator again and run wsl.exe --install Ubuntu
6. You will be asked to create a Username and Password. The Password will not be visible to you when you're typing so be careful.
7. Install VSCode (skip if it is already downloaded on your system). Go to the website and run the Windows installer. When it finishes downloaded and you click on it, it will ask you for where to install etc. When the installer asks you to select additional tasks, select "ADD TO PATH."

<img width="397" alt="Screenshot 2025-01-20 at 12 37 50 PM" src="https://github.com/user-attachments/assets/411a2795-105d-47b4-bc9e-ce29b834035e" />


8. Install the WSL and C/C++ extensions from the website. (https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)-> search C/C++ on the same website. 
9. Click install and it will ask you to open VSCode. Allow it to open VSCode and then click Install.
10. Open WSL terminal by typing WSL in the search bar.
11. You should see username@laptopname:~$
12. Run this to update all packages: sudo apt update && sudo apt upgrade
13. After that command finishes executing, type: sudo apt install gcc
14. You're done with installation! Just run mkdir <name> to create a directory inside working directory.  Example: to make a directory called 'hello', run mkdir hello
15. To enter into that directory, run cd <name>
16. Open the folder in VS Code with code . (include the full stop)
17. VSCode would show a bunch of fetching commands- it is getting integrated with whatever you have just created.
18. In the Explorer tab, right click and select "New File" and make a new C file (example: "hii.c")



ERRORS YOU MAY ENCOUNTER:
............ in step 2. if it says "the connection with the server could not be established"
SOLUTION ----> Check your internet connection. It works on campnet- sometimes fails with JIO. Don't worry, this is just during installation, it's a one time thing. This issue arises only during installation- it WILL work on any network after that. Reconnect to campnet/use hotspot. 
Alternatively, install Ubuntu app from Windows Store. 



............. in step 5. if it says "Ubuntu is already installed. The requested operation is successful. Changes will not be effective until the system is rebooted.", or if it says 
"Installing, this may take a few minutes...
WslRegisterDistribution failed with error: 0x8004032d
Error: 0x8004032d (null)"  
SOLUTION ----> search hypervisor in your search bar. 

<img width="554" alt="Screenshot 2025-01-20 at 12 48 15 PM" src="https://github.com/user-attachments/assets/77d95e07-e533-4d1a-aa5b-30a57b5d7cb7" />

You must enable Virtual Machine Platform feature and Windows Subsystem for Linux (all of them must be tick marked)
Restart your computer once you do this. 


