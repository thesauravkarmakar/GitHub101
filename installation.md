## Installation Steps

### For Windows

1. Download Git from https://git-scm.com/downloads 
2. Run the installer program, follow the defaults.
   :zap: Tweak 
   
   
    <img src="https://github.com/thesauravkarmakar/GitHub101/blob/master/images/git.PNG">
3. Git requires your name and email address before you do any of your work. It is best to just configure Git from the start.
4. Open Git Bash and enter the below mentioned code.
```
git config --global user.name "Your Name"
git config --global user.email "your.email@email.com"
```
5. Close Git Bash.

##### Notepad++
 
6. Download **Notepad++** from https://notepad-plus-plus.org/downloads/
7. Run the installer program, follow the defaults. 
8. [Add Notepad++ to system's PATH environment variable](https://superuser.com/questions/607379/how-do-i-start-notepad-from-cmd)
9. Open Git Bash and type 
```
notepad++ ~/.bash_profile 
```
10.  It will open and create **~/.bash_profile file**. Then add below mentioned line to it 
```
alias npp='notepad++ -multiInst -nosession'
```
11. Restart Git Bash.
12. To make Notepad++ default text editor in Git, type this command in Git Bash
```
git config core.editor "notepad++ -multiInst -nosession"

```
13. Then test it out by opening Git config's file  with Notepad++.
```
git config --global -e
```
_If Notepad++ close the global config file, then your Git Integration is successful._

##### P4Merge
_P4Merge for Windows which is a visual comparsion and merge resolution tool that integrates well with Git._


14. Download **P4Merge** from https://www.perforce.com/downloads/visual-merge-tool
15. Run the installer program.
16. Select *only* the Merge and Diff Tool and deselect all others.
   <img src="https://github.com/thesauravkarmakar/GitHub101/blob/master/images/p4merge.PNG">
   Accept all defaults otherwise.
   
17. Now, let's integrate P4Merge with Git. You'll need to know where P4Merge is installed on your system -- which is normally under _Program Files_
18. Configure P4Merge as ***Diff Tool** in Git:
```
git config --global diff.tool p4merge
git config --global difftool.p4merge.path "C:/Program Files/Perforce/p4merge.exe"
git config --global difftool.prompt false
``` 
19. Configure P4Merge as **Merge Tool** in Git:
```
git config --global merge.tool p4merge
git config --global mergetool.p4merge.path "C:/Program Files/Perforce/p4merge.exe"
git config --global mergetool.prompt false
```

### For Linux

1. Git can usually be installed via the package manager used by your linux distribution ,to install git for your linux system run the following command in your terminal, depending on the distribution you are using.  

For Ubuntu, Debian and distributions based on them  
```
sudo apt install git  
```  
For Arch, Manjaro and other Arch based distributions  
```
sudo pacman -S git
```  
For Fedora,CentOS and RHEL
```
sudo dnf install git
```
For OpenSUSE 
```
sudo zypper install git
```
2. Follow steps 3 and 4 mentioned in the Installation for windows to configure git.
### :white_check_mark: You are done with the installation! 

### For macOS

Method 1: Installing GitHub Desktop

GitHub Desktop simplifies the development workflow with a UI. It will install Git if your system doesn't already have it.

1. Download GitHub desktop from https://desktop.github.com/
2. Follow the instructions in the installation window. You'll need a GitHub account.
3. Once installed, check yout Git version with:
```
git --version
```

Method 2: Using Xcode

Apple ships Git as part of their Xcode commmand-line tools.

1. Open **Terminal** and run the following command:
```
xcode-select —install
```
2. A new window will pop-up asking you if you want to install Xcode command line developer tools, select yes
3. Once the installation finishes, you can check your Git version in Terminal with:
```
git --version
```

Method 3: Using Homebew

Homebew is a popular method for downloading software

1. Open **Terminal**
2. Run the following command:
```
brew install git
```
3. If you dont have brew already installed, you can install it with this command:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
4. Once Brew is installed and you run step 2, check your Git version with:
```
git --version
```
