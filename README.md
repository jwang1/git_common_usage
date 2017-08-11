# git_common_usage
notes for git usage, common commands

1. Push local git repository to GitHub

   1.1 Create a GitHub repository, 
   
   1.2 Get its clone url
   
   1.3 git init  local git-repository
   
   1.4 *git remote -v*   (there will be empty, for a newly created local-git-repo which is not linked to remote repo yet)
   
   1.4 ```git remote add github-remote-url``` 
   ~~1.4 git remote set-url origin github-repository-url~~
   
   1.5 git remote -vv  (now should see the remote-github-url)
   
      1.5.1  ```git branch --set-upstream-to=origin/master master```  (set local master branch to track remote github master branch)
      
      1.5.2  ```git branch -vv``` (can tell if local master branch links/tracks remote-github-repo-master-branch)
      
      1.5.3  ```git pull --rebase``  (will get code from remote-master-branch, and put local changes on top of that - rebase)
   
   1.6 git pull --rebase  (supposedly using default master branch),  to get remote repository README.md etc
   
   1.7 ```git push --set-upstream origin master```  (upload local git-repository to GitHub)
   
   *Reference:* 
   
    Add remote-url: 
    
       https://help.github.com/articles/adding-a-remote/
   
    Change remote-url for local repo: 
    
       https://help.github.com/articles/changing-a-remote-s-url/
   
2.    
