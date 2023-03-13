---
tags: Projects, Josh, ObsidianCollaborate
---

# Goal state 

Create a process for this: 

(1: obs: don) => (2: folder:don local) => (3: github: don) => (4: github: linda) => (5: folder: linda local: modify) => (6: github: linda to don) => (7: folder: don local) => (8: obs: don)

# 1. GitHub Repo

Setup a new repo H3 on git; add the README.md file
Get the address so I can clone it. 
https://github.com/delger/H3.git

# 2. To Local Repo To GitHub

Create a local repo by cloning remote repo
```
(base) $ cd /Users/donaldelger/Desktop
(base) $ git clone https://github.com/delger/H3.git
```
Add project files to the Local Repo

Enter the following commands:
```
$ cd H3
$ git add -A
$ git commit -m "Added project files"
$ git branch
$ git remote -v
$ git push origin main
    - enter my user name
    - enter my personal access token
```
# 3. Collaborator Forks the Repo

Linda logs into github
Linda searches for "delger/H3" and clicks on the directory
Linda clicks on the fork button

# 4. Collaborator Clones the Repo

Linda clicks on the green Code button and copies the URL.

On her computer, Linda navigates to parent directory that will hold the local repo.
Then, Linda clones the fork as follows:     
`git clone https://github.com/LindaElger/H3.git`

# 5. Collaborator Makes Changes and Uploads to Her Git Hub

Linda changes shared files. 
```
$ git add -A
$ git commit -m "Added exercise info; tahiti info"
$ git push origin maim
```
As usual, Linda needs her user name and PAT (personal access token).

# 6. Linda Makes a Pull Request to Don

Click pull request. 

# 7. Don Responds to the Pull Request

Don gets an email or Don goes to GH

Merge the pull request. 

# 8. Don pulls the changes from the remote repo to his local repo. 

Navigate to local repo directory. 
`git pull`

Now I have all of Linda's changes. 
