# IDE - SEZER AKSOY FAF-151

## 1. Preparing Process for This Laboratory Work.
In order to connect to remote server we have to make one. So just we need to install virtual box for this. 
After installing Virtual Box we have to download and install linux operation system. I’ve chosen Ubuntu for that.

## 2. Connect via ssh
We can find our virtual ubuntu’s ip address with this commond: ifconfig
And after find our ip address then we should check our connection status with ping you should see the following screen.

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/1.PNG)

We can connect to our server via SSH such like following:

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/0.PNG)


## 3. Run Simple Programs 
Firstable we should install same necessary compiler on our Ubuntu. I will install  “gcc” and “g++” with following commands
sudo apt-get install gcc
sudo apt-get install g++


Run programs with the following commands:
gcc hello.c –o hello
./hello

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/2.PNG)

g++ hello.cpp –o hello2
./hello2

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img3.PNG)

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/4.PNG)


## 4. Set-Up Git
First of all we have to install git sudo apt-get install git
Configure global user name git config --global user.name "szraksy"
Configure global user email git config --global user.email "aksoysezer95@gmail.com"
Initialize git repo git init
Generate ssh key with ssh-keygen
Set the public key in github

## 5. Creat New Branches

Add two new branches with git branch nameOfBranch
Move to new branch with git checkout nameOfBranch
Now we can commit to a new branch
If we want to move back or to another branch use again git checkout anotherBranchName
This is how it looks in command line:

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/6.PNG)

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/7.PNG)



## 6. Add files to Git
We are adding our files to git with following commond:  git add ./filename

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/8.PNG)

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/9.PNG)




We have 3 differents branches so I will add my files also to the another branch

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/10.PNG)

## 7. Tracking, reset and merging

To reset branch to previous commit use git checkout e48215c6ec4cd8305988bea9ae4ec68d755047d7

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/11.PNG)

Merging of two branches is done with git merge nameOfBranchToMergeCurrentOne

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/12.PNG)

## 8. Git Branching –Rebasing

In Git, there are two main ways to integrate changes from one branch into another: the merge and the rebase. In this section you’ll learn what rebasing is, how to do it, why it’s a pretty amazing tool, and in what cases you won’t want to use it.

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/13.png)
The easiest way to integrate the branches, as we’ve already covered, is the merge command. It performs a three-way merge between the two latest branch snapshots (C3 and C4) and the most recent common ancestor of the two (C2), creating a new snapshot (and commit).

![Alt] (https://github.com/szraksy/IDE/blob/master/LAB1/img/14.png)

However, there is another way: you can take the patch of the change that was introduced in C4 and reapply it on top of C3. In Git, this is called rebasing. With the rebase command, you can take all the changes that were committed on one branch and replay them on another one.
In this example, you’d run the following:
$ git checkout experiment
$ git rebase master

## Conclusion
When we are working on a project I thing big problem is connection to your project from everywhere and by your collogue. So this laboratory work helped us to find a solution how we should keep our project files online and to the remote server. 
And the most beautiful advantage with GIT everyone work on the same project at the same moment but nobody lost and files or coding with this way.
VCS is a wonderful tool which allow you to control your project, work with a team of developers and to track all the changes which was ever made. We've set a good background on VCS and Git in particular.
So we have a lot of stuff to learn with this way and with this laboratory works.
