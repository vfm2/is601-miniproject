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

### Remote (Add / Remove / Show)

**Definition:** Remote as its own command deals with keeping track of repositories and branches being worked on.
However, what we are interested in are three arguments that are used with remote: add, remove, and show.
* Add: The add argument can be used for adding repositories to your machine.
* Remove: The remove argument is the opposite of add, and deletes any repositories from your machine.
* Show: The show argument provides information on the specified repository (origin is the default).
Such information includes the repo URL and any remote or local branches. 


**Example:**
````shell
git remote add newRepo <url>
#This command takes the Git repository provided in the URL, and adds it to your local machine under the name newRepo.

git remote remove newRepo
#This command will remove the newRepo repository on your local machine. Everything that was on that repo will also be removed.

git remote show origin
#This command shows plenty of information on the origin repository.
````


### Status

**Definition:** Status is used to check on information about the branch you are currently working on.
This command has no effect on anything you modify and only outputs information. 
It is often used to check what branch you're working on and see what files haven't been committed (and pushed) yet.
Information that the output gives you includes the following:
* Current branch
* Modified files that haven't been committed
* Modified files that haven't been staged
* If branch is up to date with the repository
* If there is any conflicts in files when attempting to merge

**Example:**
````shell
git status
#This command gives all the information defined above.

git status -s 
#This command gives the same output as above but in a more concise and shorter format.
````

### Master Branch

**Definition:** The Master Branch is the branch that has all of the most updated code and programs.
It is the default branch in the repository and is also sometimes called the main branch.
Developers will normally create their own branches to contribute work, and that work gets updated to the master branch.
The master branch contain all of the newest and best changes after having code pushed into and pulled from other branches.

**Example:** This is an example visualization of what the master branch and other branches look like when using Git.
There are two branches in which work is completed, but whatever changes are made in those two branches will eventually
be pushed back into the master branch and pulled by the master branch.

![Image of Master Branch](https://static.javatpoint.com/tutorial/git/images/git-branch.png)

#### Previous Page: [Gitflow](https://github.com/vfm2/is601-miniproject/blob/main/gitflowPage.md)
#### Back to [README.md](https://github.com/vfm2/is601-miniproject/blob/main/README.md)

##### [Top of page](#Git-Terminology) &#8593;



