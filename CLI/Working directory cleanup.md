# Git repository cleanup

After adding **.gitignore** file command `git ls-files -z --ignored --exclude-standard | xargs -0 git rm --cached` followed by `git commit -m "Repository cleanup adter adding .gitignore"` can be used to delete all committed files from git. 

Those commands create a commit which deletes all ignore files from git. Files will remain in git history but are not present in future commits.

# Deleted file recovery

Command `git log --all --pretty=format: --name-only --diff-filter=D -E  $COMMIT -- *.user` lists all deleted .user files in given commit.

Deleted files can be recovered from given commit into workspace with
`git log --all --pretty=format: --name-only --diff-filter=D -E -z $COMMIT -- *.user | xargs -0 git restore --source=$COMMIT^ -W --` where COMMIT is commit that deleted files. 

Running the command recovers files into working directory. `*.user` is example here and can be replaces with given set of files.