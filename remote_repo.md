Hello , so you must be wondering what a remote repository is . Let me explain : A remote in Git is a common repository that all team members 
use to exchange their changes. In most cases, such a remote repository is stored on a code hosting service like GitHub or on an internal server.
In contrast to a local repository, a remote  does not provide a file tree of the project's current state but only consists of the .git versioning data.


Now , to setupa remote repository , follow the given instructions :-
To add a new remote, use the git remote add command on the terminal, in the directory your repository is stored at.

The git remote add command takes two arguments:

A remote name, for example : origin
A remote URL, for example, https://github.com/user/repo_name.git
For example:

$ git remote add origin https://github.com/user/repo.git
# Set a new remote

$ git remote -v
# Verify new remote
> origin  https://github.com/user/repo.git (fetch)
> origin  https://github.com/user/repo.git (push)

