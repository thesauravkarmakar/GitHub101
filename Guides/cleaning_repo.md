# Cleaning a Repository

### Whenever we are working on a project, there certain files which we wish not to keep track of. For instance, log files, compiled code ( .class, .oc files), dependency caches (such as /node_modules) etc. 


### Thus it is important to ignore such files as this cleans up our repository and makes collaboration easier and faster.

### We can ignore such files using ``` .gitignore```.

### ```.gitignore ``` file keeps track of all the files that we wish to ignore.


### These are usually stored at the root of the repository

### Suppose your directory has a file ```main.cpp```. On compiling the code, it generates an ```a.out``` file. 

### On doing ```git status```, you will notice that ```a.out``` is one of the untracked files. (as we have not commited it yet)

![image](https://user-images.githubusercontent.com/38832512/96430171-761f9700-121f-11eb-930a-5f6e3f2ee6d0.png)

### To ignore the ```.out``` file, create a ```.gitignore``` file and add *.out. This tells it to ignore all files of the extension .out

### This is what the gitignore file looks like

![image](https://user-images.githubusercontent.com/38832512/96432369-68b7dc00-1222-11eb-9319-84ff603264b7.png)


### After adding the ```.gitignore``` file, this is what the repo status looks like

![image](https://user-images.githubusercontent.com/38832512/96430528-e6c6b380-121f-11eb-8118-452ca01458b8.png)


### This helps in cleaning up the repository and making sure we don't have unwanted files in our directory. 

### The same can be done for folders.
### Just add a ``` /node_modules ``` in your gitignore file, and that will do the job.



