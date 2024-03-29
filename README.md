# Git Commands

<img src="https://github.com/stefgina/git-commands/blob/main/git.png" height=110 width=320>

Most usual command sets:

1. contribute to repo
2. start a repo and publish on github
3. contribute to an existing branch on github

## 1. Contribute to an existing repository
```
# download a repository on GitHub.com to our machine
git clone https://github.com/me/repo.git

# change into the `repo` directory
cd repo

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make changes, for example, edit `file1.md` and `file2.md` using the text editor

# stage the changed files
git add file1.md file2.md

# take a snapshot of the staging area (anything that's been added)
git commit -m "my snapshot"

# push changes to github
git push --set-upstream origin my-branch
```

## 2. Start a new repository and publish it to GitHub
```
# create a new directory, and initialize it with git-specific functions
git init my-repo

# change into the `my-repo` directory
cd my-repo

# create the first file in the project
touch README.md

# git isn't aware of the file, stage it
git add README.md

# take a snapshot of the staging area
git commit -m "add README to initial commit"

# provide the path for the repository you created on github (you must create the repository on github website first!!)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git

# push changes to github.
# if that fails you should propably change main to master, since thats the old way of doing it.
git push --set-upstream origin main
```

## 3. Contribute to an existing branch on GitHub
```
# assumption: a project called `repo` already exists on the machine, and a new branch has been pushed to GitHub.com since the last time changes were made locally

# change into the `repo` directory
cd repo

# update all remote tracking branches, and the currently checked out branch
git pull

# change into the existing branch called `feature-a`
git checkout feature-a

# make changes, for example, edit `file1.md` using the text editor

# stage the changed file
git add file1.md

# take a snapshot of the staging area
git commit -m "edit file1"

# push changes to github
git push
```

## 4. Random Sets
```
# delete ds store
find . -name ".DS_Store" -delete

# delete hidden folder
rm -rf .hiddenfolder

# todo more rans

```
