GIT:

	GIT LOG:
		I want to check the difference of each file (-p) for the last 2 commits (-2).
			$ git log -p -2  
		I want to check an specific file and how many lines where updated in each commit.			
			$ git log --stat  
		I want a pretty way to see commits
			$ git log --pretty=format:"%h - %an, %ar : %s" 
		I want to see the commits with the branches structure. 
			$ git log --graph 
		I want to check the commits that were made the last 2 weeks avoiding merges commits.
			$ git log --since=2.weeks --no-merges
		
	GIT AMMEND:
		Ops, I forgot to add a file and/or I want to change a typo. If you have your changes LOCALLY ->
			1. git commit -m 'Initial commit'
			2. git add forgotten_file
			3. git commit --amend
		Ops, I add a file that I don't want in the commit
			$ git reset HEAD <file.name> or $ git restore --staged <file.name>
		Ops, I don't want to commit neither stash the changes that I made in <file>. Unrecoverable!
			$ git checkout -- <file.name> or $ git restore <file.name>
			
	GIT REMOTES:
		I want to clone a remote repository.
			$ git clone <http url or ssh>
		I want to upload my repo to github.
			$ git remote add upstream <url.git>
		I want to check the contributors of this repo.
			$ git remote -v
		
			
			
			
		

