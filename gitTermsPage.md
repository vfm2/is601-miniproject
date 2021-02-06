# Git Terminology
### Learn the basic terms for using Git!

1. [Repository](#Repository "Go to Repository") 
2. [Clone](#Clone "Go to Clone")
3. [Fork](#Fork "Go to Fork")
4. [Branch](#Branch "Go to Branch")
5. [Commit](#Commit "Go to Commit")
6. [Merge](#Merge "Go to Merge")
7. [Checkout](#Checkout "Go to Checkout")
8. [Push](#Push "Go to Push")
9. [Pull](#Pull "Go to Pull")
10. [Remote Add / Remove / Show](#Remote-Add-/-Remove-/-Show "Go to Remote")
11. [Status](#Status "Go to Status")
12. [Master Branch](#Master-Branch "Go to Master Branch")



### Repository

**Definition:**

- words

**Example:**

- words



### Clone

**Definition:**

- words

**Example:**

- words



### Fork

**Definition:**

- words

**Example:**

- words



### Branch

**Definition:**

- words

**Example:**

- words



### Commit

**Definition:**

- words

**Example:**

- words



### Merge

**Definition:**

- words

**Example:**

- words



### Checkout

**Definition:** Checkout is used for preparing to work on a specific branch. You often use _git checkout_ when you want to
work on some code that isn't on the main branch. You can use this command to switch to an already existing branch
or even make a new branch, then switch to that branch to work on.

**Example:**
```shell
git checkout foo 
#This command switches to already-exiting branch named foo.

git checkout -b notMain
#This command makes a new branch named notMain and switches to it.
```

### Push

**Definition:** Push is used to upload any changes made on a local machine or repository
onto the main/master repository. It is often known as the opposite of _git fetch_. Once those changes are
pushed onto the main repository, other collaborators are able to see those changes you made on your
local machine/repository. With this command, you specify from what branch you are pushing from and onto where
(normally the main). What's also good about this command is that unless you force it to, it will not 
overwrite anything that is in the main branch.

**Example:**
```shell
git push 
#This command updates changes to the main branch.

git push foo main
# This command more speciically updtates changes to the main branch from the foo branch.

git push -f 
#This command forces a push that may  normally be blocked by git.

git push -all 
#This command updates changes to the main branch from all other branches.

```

### Pull

**Definition:** Pull is the opposite of push. It is used to download updates or changes from one branch to another. 
You can pull changes from some remote branch into your local branch or vice versa.
This is also key in ensuring the main branch is updated with changes from your own branches.
On GitHub, you can also use Pull Requests. Pull is also a combination of fetch and merge.

**Example:**
````shell
git pull 
#This command is the default for fetching changes from the master branch onto your local branch.

git pull --rebase
#This command pulls all changes from the main branch and any local changes are applied on top of the main changes.

git pull origin master
#This command pulls changes from the master branch into the origin branch.
````

### Remote Add / Remove / Show

**Definition:**

- words

**Example:**

- words



### Status

**Definition:**

- words

**Example:**

- words



### Master Branch

**Definition:**

- words

**Example:**

- words



##### [Top of page](#Git-Terminology) &#8593;






