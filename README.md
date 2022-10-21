## git config
    git config –global user.name “[name]”
  
    git config –global user.email “[email address]”
  
## init
    git init [repository name]
  
## clone
    git clone [url]
    
    git clone --branch <branchname> <remote-repo-url>  -> for specific branch
    
    or 
    
    git clone -b <branchname> <remote-repo-url> 
  
## add
    
    send file to staging area(green color) for commit
    
    git add . -> all file
    
    git add file_name -> for specific file
  
 ## commit
    git commit -m “commit message”
    
    git commit -a -m "message" -> skip staging area and commit all file
  
 ## pull
    git pull 'remote_name' 'branch_name'
  
 ## push 
    git push 'remote_name' 'branch_name'
  
## branch
    git branch -> lists all the local branches in the current repository
  
    git branch [branch name] ->  creates a new branch
  
    git branch -d [branch name] -> deletes the feature branch.
  
    git checkout [branch name] -> used to switch from one branch to another.
  
    git checkout -b [branch name] -> creates a new branch and also switches to it.
  
    git merge [branch name]-> merges the specified branch’s history into the current branch
    
## swicth b/w branch

    git checkout branchname
    
    or 
    
    git checkout branchname
  
  
## commit info
    git log  -> all commit info
    
    git log -p -n -> to see last n commit
    
    git commit --amend -m "New commit message"
    
    
  ## diff
    git diff -> shows the file differences which are not yet staged.
    
    git diff –staged  -> shows the differences between the files in the staging area and the latest version present
    
    
  ## match data with last commit
      git checkout -f -> for all file
      
      git ckeckout file_name -> match that file to last commit
      
      
      
  ## delete 
      git rm file_name  -> delete
      
      git rm --cached fie_name  -> remove from staging area and send it to untracked file
      
      
  ## list all file 
      ls
     
      
  ## short status
      git status -s
      
  ## ignore file (.gitignore)
      touch .gitignore -> create file (contains untracked file)
      
      *.log -> add this line to .gitignore file if u want to ignore all log file
      
      *.py -> add this line to .gitignore file if u want to ignore all python file
      
      folder_name/ -> to ignore this folder
      
      
      
  ## stash
  
    u have done some changes and now u want to pull code, but u don't want to remove ur changes before taking pull and write again 
    after taking pull so, in this case u can stash ur file
    
    git stash -> command temporarily stores all the modified tracked files.

    git stash -m "name"  -> to give name
    
    and after pull u can want back ur changes
    
    git stash list  -> lists all stashed changesets
    
    git stash apply   -> apply last stash 
    
    git stash apply stash@{2}   -> apply specific stash
    
    git stash pop  -> delete last stash
    
    git stash drop stash@{2}  -> delete specific stash
    
    git stash clear  -> delete all stash list
    
    git stash branch "branch name" stash@{2}  -> create branch from stash 
    
    
    
  
    
    
      
  
  
  
  
  
  
