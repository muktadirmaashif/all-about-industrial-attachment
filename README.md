# This is a step by step procedure on how to setup WSL 2 on Windows
* All commands of windows needs to be executed in powershell (Administrator)

## In newer windows versions, you just have to type in  - 
```
wsl --install
```

## For manual installation

1. In Windows, search for "Turn windows features on or off."
2. Check "Windows Subsystem for Linux" option

### WSL 2 update:
there are some requirements for updating wsl version 2. I guess all of them are met in newer versions of windows. If you want, you can check them [here](https://docs.microsoft.com/en-us/windows/wsl/install-manual)

3. Enable Virtual Machine option in "Turn windows feature on or off"
4. Go restart your machine. This tutorial will be right here for you!

5. Download Linux Kernel update from [here](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) and install it. 

6. Set WSL version 2 as default - 
```
wsl --set-default-verion 2
```

7. Install your Linux distro of your choice. (Ubuntu ofviously! I know, right? :p) I am recommending LTS version. Your will find them in Microsoft Store. 

8. First time openning, you will have to state your username and password. Go do that. 

9. type in your ubuntu terminal - 
```
sudo apt update && sudo apt upgrade
```

At this point, your ubuntu wsl is ready to roll! Let's move in to the next part where we will use VC Code to work on a project. 

---

## Configuring VS Code with WSL

1. Assuming you have VS Code installed in windows, open it and search for 'WSL-remote' in Extension marketplace. 
2. Install it. It is an extension by Microsoft that will enable working with wsl.
3. Check bottom left corner of the panel. You should see a small green icon. if you can't, press ctrl+shift+p to open command palette of VS Code, and search for 'Remote-wsl.' Select it. 
4. Press ctrl+` (it is called backtick and you will find it just above the tab key) to open integrated terminal. 

That's it! You are all set. Start doing your magic. Happy coding!  
