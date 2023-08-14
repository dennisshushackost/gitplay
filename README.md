# Summary of the commands in this Tutorial:

````
```bash
# Get git:
sudo apt-get update && sudo apt-get install git

# Get the current version:
git --version

# Configure git:
git config --global user.name John Doe
git config --global user.email john.doe@ost.ch
git config --global core.editor nanogit --version

# Initalise a git repo: (.git) is created
git init

# Check the status:
git status 

# Add files: (Changes to be commited)
git add text1.txt

# Add a commit: 
git commit -m "My first commit"
Nothing to commit left

# shows the logs of the commits
git log 

# Show contents at this commit 
git show 3c6c42b3c38e4ba38f5d9de6a229d09d0a982155:text1.txt

# Show differences in files:
git diff 7879b233cfcffed19d5c874b8670cccb31e53ca5 6aaba06df0990bb79cf0ead11e0367215778e2df
git diff 7879b233cfcffed19d5c874b8670cccb31e53ca5 6aaba06df0990bb79cf0ead11e0367215778e2df

# Going to the latest commit
git checkout master

# Going to a previous commit state
git checkout 3c6c42b3c38e4ba38f5d9de6a229d09d0a982155

## Branching 

# Creating a branch and switching to this branch (-b = new branch)
git checkout -b test
git checkout master

# Show all branches:
git branch

# Show the log
git log --all --decorate --oneline --graph

# Merging:
git checkout master
git merge test
```