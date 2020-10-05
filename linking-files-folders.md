1) Make sure `git` is installed on your system.
2) Using your command line, get inside the folder where your project files are kept by `cd/path`
3) Check if git is initialized: `git status`
If you get this error message: `fatal: Not a git repository (or any of the parent directories): .git`this means the folder you are currently in is not being tracked by `git`

**Create an EMPTY REPOSITORY on GitHub**
1) Login to your [GitHub](www.github.com) account.
2) At the top right you will see a '+' icon. Click on that and then select 'New Repository'
!['New Repository'](https://drive.google.com/file/d/12BTp3EVHC42UM2-i0jBQrz6_mETUxdTH/view?usp=sharing)
3) Give your repository a name, probably the same name as your local project.
!['Create Repository'](https://drive.google.com/file/d/1Ta7pB_tzPte66_uG9YucUandrIuMW1gP/view?usp=sharing)
4) Click 'Create Repository'.
![Name the repo](https://drive.google.com/file/d/1TPC9QgHdMBlI2dH0H44l80CGCKa3knYI/view?usp=sharing)

**Connect your local project folder to your empty repository on Github**

The screen visible to you now on Github is titled 'Quick setup — if you’ve done this kind of thing before'.
1) Copy the link in the input right beneath the title, it should look something like this: https://github.com/rashipathak/repo-name.git This is the web address that your local folder will use to push its contents to the remote folder on Github.
2) Go back to your project in the command line.
3) In your command line, type `git remote add origin [copied web address]`
For example: `git remote add origin https://github.com/rashipathak/repo-name.git`
![image](https://drive.google.com/file/d/1EBokjp5RX3Dj3w0NPGC1tOt_oaI2jAtS/view?usp=sharing)
4) Push your branch to Github by `git push origin master`
5) Go back to the repository screen on Github that you just left, and refresh it. The title 'Quick setup — if you’ve done this kind of thing before' will disappear, and you will see your files there.
