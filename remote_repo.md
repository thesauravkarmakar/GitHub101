**GUIDE TO CREATE A REMOTE REPOSITORY**

Hello , so you must be wondering what a remote repository is . Let me explain : A remote in Git is a common repository that all team members 
use to exchange their changes. In most cases, such a remote repository is stored on a code hosting service like GitHub or on an internal server.
In contrast to a local repository, a remote  does not provide a file tree of the project's current state but only consists of the .git versioning data.


**Now , to setup a remote repository , follow the given instructions :-
To add a new remote, use the git remote add command on the terminal, in the directory your repository is stored at.

**The git remote add command takes two arguments:

**A remote name, for example : origin
A remote URL, for example, https://github.com/user/repo_name.git

For example:

<img width="458" alt="Screenshot 2020-10-20 at 9 39 42 AM" src="https://user-images.githubusercontent.com/58665834/96539295-5be5c780-12b8-11eb-840e-ca54b6fdaf7f.png">


**Set a new remote

$ git remote -v

For Example :-

<img width="458" alt="Screenshot 2020-10-20 at 9 42 31 AM" src="https://user-images.githubusercontent.com/58665834/96539416-9bacaf00-12b8-11eb-8fa7-973fb738de4d.png">


**Verify new remote

 origin  https://github.com/user/repo.git (fetch)
 origin  https://github.com/user/repo.git (push)


For example :-


<img width="458" alt="Screenshot 2020-10-20 at 9 43 55 AM" src="https://user-images.githubusercontent.com/58665834/96539499-c8f95d00-12b8-11eb-9e0d-24a83d436631.png">


**To check all your remote repositories type : git remote 

For example :-


<img width="458" alt="Screenshot 2020-10-20 at 9 46 45 AM" src="https://user-images.githubusercontent.com/58665834/96539636-2d1c2100-12b9-11eb-9e42-d666d0c57ac4.png">


**After typing git remote , you should see the below 

<img width="458" alt="Screenshot 2020-10-20 at 9 48 37 AM" src="https://user-images.githubusercontent.com/58665834/96539750-6e143580-12b9-11eb-8ed0-74a2a55120e7.png">


As you see , if you find your remote name in the list , you have successfully created a remote repository .

Hope , this helps you , all the best and happy coding .
