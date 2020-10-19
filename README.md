# git-commands
Essential and all major git commands.

GIT Commands

Git Basic Commands :

1.	git init = create local repositories
2.	git add file(s) = add file to stagging area for commit changes or add files to index
3.	git status = shows difference between stagging area and working area before commiting
4.	git commit = commit changes to index from stagging area and put into local repository
5.	git push = push files to remote repository
6.	git pull = get latest changes from remote repository
7.	git clone = copy remote repository to local device

Git Extended Basic Commands :

1.	git --version = get git version
2.	git config --global user.name 'san' = add user name
3.	git config --global user.email 'mail@example.com' = add user email
4.	git add index.html = adds index.html to stagging area
    when call git add command this will add default option as -A or --all i.e., git add -A or git add --all
    git add command is same as git add -A command
5.	git status = get status of tracked and untracked files
6.	git rm --cached index.html = remove from stagging area to working area
7.	git add *.html = adds all html files to stagging area
8.	git add . = adds all files in current directory to git repository
9.	git add = adds all files in current directory but also adds all other directories in git repository
10.	git add -A = adds all files in current directory but also adds all other directories in git repository
11.	git add --all = adds all files in current directory but also adds all other directories in git repository
12.	git add -A directory_name = adds all files in specified directory and but not all other directories in git repository
13.	git add directory_name = adds all files in specified directory and but not all other directories in git repository
14.	git add --no-all directory_name = adds all files in specified directory and but not all other directories in git repository and ignores deleted files for stagging
15.	git add --ignore-removal directory_name = adds all files in specified directory and but not all other directories in git repository and ignores deleted files for stagging
16.	git add -u = adds deleted and modified files to stagging area but not untracked files or new files
17.	git add --update = adds deleted and modified files to stagging area but not untracked files or new files
18.	git add -u directory_name = adds deleted and modified files in specified directory to stagging area but not untracked files or new files
19.	git add * = adds only visible files to stagging area but not deleted and hidden files to stagging area
    * is shell command that mensions show all list available that why it works like this
20.	git reset = reset the all files as unstagged that was stagged before by add command
    once file changed in stagging area it shows file gets modified and say to add again to stagging area
    to add file again stagging area use git add command again
21.	git commit = commit all stagging area files to repository and git status shows nothing in working area
22.	git commit -m 'message' = commit with message directly without edit message file
    .gitignore = ignore files and folder that would not to be in repository
23.	git branch 'login' = create new branch for new working module that not affected to master until merge
    for individual who have assigned modules and work with individual branches to complete module fully finished
    then only it is perfect to merge to master
    branch files never shows another branch files except master
24.	git checkout login = switch from master to login branch
    once switched the files in from branch disappears and shows only switched branch
25.	git merge login = merge login branch to master
26.	git remote add origin repository_url = add remote repository_url to local git
27.	git remote = check list of connected remote repository
28.	git push -u origin master = add local to remote repository
29.	git push -f -u origin master = add local to remote repository with forced
30.	git push = add changed local commit to remote repository and not all files again
31.	git clone remote_repository = clone or copy remote repository to local device
32.	git pull = get all changes done by all other developers working on same project to local device
33.	git push origin = add local branch to remote origin
34.	git push origin branchname = add local branch to remote repository branch

Git Extras Commands:

1.	git diff = check and show the difference of changes in local repository
    + symbol shows added files
    - symbol shows removed files
2.	git commit filename -m 'message' = commit the changes made with in filename but not others
3.	git log = get all changes done in git commit
4.	git config user.name 'username' = adds another username
5.	git config --global user.name 'username' = created global username
6.	git log --oneline = show all changes done in one line
7.	git branch -d branchname = delete branch
8.	git diff filename = check and show the difference of changes in filename
9.	git checkout . = revert all file changes to last before one commit
10.	git checkout commit-id = revert all file changes to the commit id
11.	git checkout master = revert all file changes to after checkout specific commit-id
12.	git reset --hard commit-id = hard delete all changes made on commit id and cant revert back by checkout. before use hard reset execute carefully

Git Stash Commands :

1.	git stash = save all recent changes to temperary storage and revert files back to last known commit
2.	git stash save "message" = save all recent changes to temperary storage and revert files back to last known commit with recent message
3.	git stash list = get list of all stash
4.	git stash apply = apply saved last created stash to working directory and stash will exist there.
5.	git stash apply stash-id = apply saved stash-id to working directory and stash will exist there.
6.	git stash pop = apply saved last created stash to working directory and applied stash will dropped.
7.	git stash pop stash-id = apply saved stash-id to working directory and applied stash will dropped.
8.	git stash drop stash-id = drop the stash-id
9.	git stash clear = drop all stash
    all stash exist among all branches

Git Commands for log/report/information about repository :

1.	git log = shows all commits made on repository
2.	git log --online = shows all commit in one line
3.	git log --graph = shows all commit in graph structure
4.	git log --graph --oneline = shows all commit in oneline graph structure
5.	git log --stat = shows all commit with changed lines
6.	git log -p = shows all commit with what content has changed with detailed like diff command for individual commits
7.	git log -5 = shows last 5 commits
8.	git shortlog = shows all commit made sorted by authors by default
9.	git shortlog -n = shows all commit made sorted by authors and no.of commits in ascending
10.	git shortlog -s = shows all quantity of commit for individual author
11.	git shortlog -e = shows all commits of author with their email id
12.	git log --author="author-name" = filters commits by authors name
13.	git log --grep="keyword" = filters commits by matched keyword
14.	git log --pretty=format:"%H" = shows only commit hash only in log result
15.	git log --pretty=format:"%h" = shows only shorten commit hash only in log result
16.	git log --pretty=format:"%cn %H" = shows only commit hash id with commiter author name in log result
17.	git log --pretty=format:"%Commiter name : cn commit SHA1 hash : %h" = shows only commit hash id with commiter author name and given text in log result
18.	git log --pretty=format:"%Commiter name : cn commit SHA1 hash : %h commit date : %cd" = shows only commit hash id with commiter author name and commit date also given text in log result
19.	git log --merges = shows all merges in repository
20.	git log --no-merges = shows all commits except merges in repository
21.	git show commit-id = shows detailed changes maded in commit-id
22.	git status -v = shows detailed changes made in working area after added to stagging area

Git Reflog Commands :

1.	git reflog = shows all changes made in local repository as history and it can be revert back again
2.	git reflog show branchname = shows all changes made in branchname and it can be revert back any of changes using SHA1 Hash id
    git reflog only works on local device or local repositories only but not on remote repository
    it stores all history upto 90 days and it will no longer available after that
    it shows history and use that history id to revert that state using reset command
    It only useful for local repositories

Git reset commands :
    1.	git reset = reset/removes last commit in repository and reset files in stagged area but not reset files changes in working area
    2.	git reset --mixed = reset/removes last commit in repository and reset files in stagged area but not reset files changes in working area
    3.	git reset commit-hash = reset/removes commit-hash in repository and reset files in stagged area but not reset files changes in working area
    4.	git reset --soft = reset/removes last commit in repository but not reset files in stagged area and reset files changes in working area
    5.	git reset --hard = reset/removes last commit in repository, reset files in stagged area and reset files changes in working area, so removes and reset files as in last commit id before commit
    6.	git reset HEAD~5 = reset/removes last 5 commits in repository
    it is preferred to reset in personal branches or own commits and it may lead to collapse whole repository so, use it carefully
    default reset is --mixed

Git revert commands :

1.	git revert HEAD = reverts last commit changes and creates new commit of reverted changes
2.	git revert commit-id = reverts commit-id changes and creates new commit of reverted changes
    it is safe to use and reverts whatever commit maded and creates that previous state files as new commit in top of history
    it reverts only one commit at time
    it is opposite to reset command

Git Commit Commands :

1.	git commit --amend = modifies information of very last commit and creates new commit-id
2.	git commit --amend --author="author-name " = modifies information and author information of very last commit and creates new commit-id
    > use this --amend with causion and it modifies commit information

Git cherry-pick commands :

1.	git cherry-pick commit-id = it invokes commits from another branch having commit-id mentioned to current checkout/working branch and makes commit
2.	git cherry-pick --no-commit commit-id = it invokes commits from another branch having commit-id mentioned to current checkout/working branch and makes files changes without commit those changes
    cherry-pick copy the commit from one branch to another branch before do cherry-pick made carefully
    some times, it is useful to copy commit from feature branch to master branch, at that time use cherry-pick

Git Garbage Collection Commands :

1.	ls .git/objects/pack = it has archieved files inside that is garbage
2.	git gc = git garbage collection makes archive those unwanted objects, unreachable objects and cleans reflog
    garbage collection makes git repository smaller by archive unwanted objects

Git configuration commands :

1.	git config --list = shows list of configuration
2.	git config --global --list = shows list of global configuration

vim commands :

1.	touch filename = create file
2.	vi filename = edit file
3.	rm -rf filename = remove file
4.	mkdir directoryname = create folder/directory
5.	rmdir directoryname = remove directory
6.	cd directoryname = switch to directoryname
7.	ls = list all files and folder in current directory
8.	cd .. = switch to parent directory
9.	clear = clear console
10.	cat filename = view file content

Read in my blog: https://sansglobe.blogspot.com/2020/10/git-commands.html
