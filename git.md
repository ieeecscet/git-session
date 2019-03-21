The Local Repository

The first step in using a version control system is making the actual
repository. Here, I've made a directory named 'foss-lab' and converted
it into a git repo by using git init inside the directory. This creates
a .git directory inside the repo, which store the details about the git
version control system. This directory is our local repository. I've
also made a README.md file. ![image](../Images/VCS/1.png)

The Remote Repository

The local repository exists only on my system. We need to connect it to
a remote repository, for any sort of collaboration to be possible. So, I
made an online repo at github.com. ![image](../Images/VCS/github.png)

Now we need to connect the local repo to the online repo. This is done
using the git remote command. Syntax: git remote add origin \[URL\]
![image](../Images/VCS/2.png)

Making Changes

Any new files or any changes in existing files should be added to the
local and remote repositories. This is done with the git add command.
This add the modified and new files to the staging area. Then the files
are committed with a commit message using git commit. This records the
changes in the local repo. Syntax: git add \[FILE(S)\] git commit -m
\"MESSAGE\" ![image](../Images/VCS/3.png) ![image](../Images/VCS/4.png)

Pushing Changes to the Remote Repository

The changes we committed are currently recorded in the local repository.
To push these changes to the remote repo, use git push. In the example
given below, origin is the name of the remote, and master is the name of
the branch. Syntax: git push \[REMOTE NAME\] \[BRANCH NAME\]
![image](../Images/VCS/5.png)

Comparing Previous Versions

Use the git log command to see all the previous changes with their
commit messages. ![image](../Images/VCS/6.png) Use git checkout to
revert to a previous state of the repo. Syntax: git checkout \[BRANCH\]
![image](../Images/VCS/10.png)

Merge Conflicts

The git pull command is used to update the local repo when it is behind
the remote repo. Automatic merges of changed files occur normally, but
in cases where the same lines are changed in both the repos, a merge
conflict occurs. It can be resolved by editing the conflicted files and
choosing which change to keep. ![image](../Images/VCS/7.png)
![image](../Images/VCS/8.png) ![image](../Images/VCS/9.png)
