# java
This is project is just for learning to use git and get more comfortable with git commands.

-----------------
Git main commands
-----------------

Cloning a repository:

Why: get a copy from a remote repository (e.g. from github servers) and clone to have it locally and be able to update it localy.
Command: git clone <path to repository>
Example: git clone https://github.com/ryounes/java.git

Updating locally:

So after using your favourite editor to make changes in your local repository, git provides commands for you to organize those changes as different commits.
This way you would have locally (and remotly after pushing) different versions of your modified code grouped by commits.
To look at the modified files you can do: git status
To see all the modifications done (line by line) for all the files you can do: git diff
Now to commit those changes locally:
The first thing is to tell git which are the files to include/add for this commit  y using the command git add. Example: git add README.md
You can add more than one file by doing: git add <Path to file1> <Path to file2> ...
If you want to add all the modified files you can just add all (-A) by typing: git add -A
If you added some file X and you do not want to include it anymore in those changes you can remove it by: git rm <Path to X>

Now after adding the files to commit, you would want to commit them and use a significant message to describe the commit. Example: git commit -m "Adding ActionListener to buttons"

Now you have your changes committed in your local repo. you can still add more files and commmit again etc..
Basiclly, at some point, you would want your changes to be uploaded to the remote repo and hopefully merged. You can do that by pushing your local commits to the repo.
Before pushing, you would want to pull any eventual changes that could have been done since your last pull or since you cloned the repo. This is due to the fact that it is possible that other people are making chnages and pushing them to the same repo. In order to avoid any conflicts, git asks you to pull any possible changes before pushing yours. Exmple: git pull
This would merge any eventual remote updates with your local repo. In case of merging conflicts, git would notify you to fix them before pushing. And after that, you are ready to push your changes using: git push

Next will be talking about branches and pull requests
