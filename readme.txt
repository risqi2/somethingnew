git config
git add files
git status


git commit -m "message"

if you want to skip the STAGE option
The -a option will automatically stage every changed, already tracked file
git commit -a -m "Updated index.html with a new line"
Skipping the Staging Environment is not generally recommended.
Skipping the stage step can sometimes make you include unwanted changes.

git status

git log 
To view the history of commits for a repository

to exit from : just type q


    git command -help -  See all the available options for the specific command
    git help --all -  See all possible commands
git branch (see all branches)
git branch new-branch-name (create)
git checkout branchname (move to other branch)
git checkout -b branchname
Using the -b option on checkout will create a new branch, and move to it, if it does not exist


We have the emergency fix ready, and so let's merge the master and emergency-fix branches.

* First, we need to change to the master branch:
git checkout master
git merge emergency-fix

git branch -d emergency-fix (delete branch)

------------------------------------------------------------

git remote add origin URL 
> specifies that you are adding a remote repository, with the specified URL, as an origin to your local Git repo

git push --set-upstream origin master


----------------------------------------------------------

updating files in github , then commit

-----------------------------------------------------------

PULL FROM GITHUB

git fetch origin
> fetch gets all the change history of a tracked branch/repo.

git status

git log origin/master
> double check by viewing the log

git diff origin/master
> showing the differences between our local master and origin/master

git merge origin/master
> merge our current branch (master) with origin/master

----------------------------------------------------------------
PULL FROM GITHUB

> pull is a combination of fetch and merge

make some change in github

git pull origin

----------------------------------------------------------------
PUSH TO GITHUB

*make some change in git local repo

git push origin

----------------------------------------------------------------
PULL BRANCH FROM GITHUB


make a new branch with some changes in github

git pull
* WE CAN SEE that there is a new branch available on GitHub.


git branch -a 
> the -a option to see all local and remote branches

git checkout newbranchnamefromgithub

git pull
* now WE CAN SEE the branch is up to date

-------------------------------------------------------------------
PUSH BRANCH FROM GITHUB

make a new branch and some changes , commit it

git push origin yournewbranchname

confirm the new branch from GitHub

