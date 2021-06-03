# GIT

## GIT LOG:
 - I want to check the difference of each file (-p) for the last 2 commits (-2).
	> $ git log -p -2
 - I want to check an specific file and how many lines where updated in each commit.			
	> $ git log --stat
 - I want a pretty way to see commits
	> $ git log --pretty=format:"%h - %an, %ar : %s" `
 - I want to see the commits with the branches structure. 
	> $ git log --graph 
 - I want to check the commits that were made the last 2 weeks avoiding merges commits.
	> $ git log --since=2.weeks --no-merges
		
## GIT AMMEND:
- Ops, I forgot to add a file and/or I want to change a typo. If you have your changes LOCALLY ->
	> $ git commit -m 'Initial commit' 
	> $ git add forgotten_file 
	> $ git commit --amend
- Ops, I add a file that I don't want in the commit
	> $ git reset HEAD <file.name> or $ git restore --staged <file.name>
- Ops, I don't want to commit neither stash the changes that I made in <file>. Unrecoverable!
	> $ git checkout -- <file.name> or $ git restore <file.name>
			
## GIT REMOTES:
- I want to clone a remote repository.
	> $ git clone <http url or ssh>
	
- I create a new repo in my local and I want to link it with a new repo in github.
	> $ git init
	> $ git remote add <remoteName> <url.git>
	> $ git add .
	> $ git commit -m 'Initial commit'
	> $ git push <remoteName> <namebranch>
- I want to have my own repo based on another repo just in case I messed up. ** Check this out!
	Note: First create a forke of an existing repo in github this would give you a url.git
	> $ git remote add <remoteName> <url.git>
	> $ git fetch <remoteName>
	> $ git checkout <remoteName>/<branch_name>
- I want to check what it is in a repo that I forked
	> $ git remote show <remoteName>
- I want to check witch remotes do I have
	> $ git remote -v
- I want to push commits that I have in the remote
	> $ git push <remoteName> <branch_name> 		
- Ops, I missspeled the name of my remote 
	> $ git remote rename <oldRemoteName> <newRemoteName>
## GIT TAGS :
- I want to create a tag based on release. Eg. v.0.0.1
	> $ git tag -a <release_version>
		https://git-scm.com/book/en/v2/Git-Basics-Tagging
			
			
Collaborators : 
	Alexandra Avendano
			
		

