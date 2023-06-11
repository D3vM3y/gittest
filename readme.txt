this repository is only for learning commands and git hub.

.gitignore file
>> includes files we don't want git to commit
>> #.log 
	>> the files with the ".log" ending will not be staged and therefore committed 
>> the gitignore file must be staged and committed

=== Commands ===
==General Commands==

cd
cd ..
ls
ls -a
mkdir
touch
open 

==Git Commands==
git init
>> initialises your git repository

git status
>> shows if your changes are staged or not

git add
>> adds your changes to the staging area

git add .
>> stages everything and not only one specific file or folder

git add *.html
>> wildcard command which stages only documents with the file ending of html 

git commit -m "your commit message"
>> commits your file or folder to the repository

git log
>> lists the git repository history and shows all the commits of the past

git branch "branch name"
>> "git branch newBranch" initialises a new branch apart from the main branch. Changes to the new branch will not affect the main branch as long as it is not merged into the main branch.

git checkout "branchName"
>> switching to another branch
>> git checkout master >> switches back to the main branch

git merge "branchName"
>> merges two branches
>> it is important that you are in the branch you want to merge your new brand to. If you want to merge the "updatesBranch" to the master branch, you need to checkout the master branch and then type in the command "git merge updatesBranch"

git stash
>> if you have unfinished tasks that are not staged but you need to switch the branch you can use git add and after git stash. This will save all your data without transferring it to your new branch

git stash apply
>> applies the stashed changes to your current branch

git remote
>> shows a list of existing remote repositories 

git clone "repository https address" 
>> this commands pulls down the entire project with all folders, files, and commits

git remote -v 
>> shows the https addresses of the repository 
>> it only works if you are in the repository folder

git fetch origin
>> fetches all changes made to the server since my last pull

git pull origin
>>this command will automatically fetch and merge all the changes from the remote to the current branch

git push origin master
>> pushes all your changes made locally to the origin on the server. It pushes to the origin and in there the master branch

