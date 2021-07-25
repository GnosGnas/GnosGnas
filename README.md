# To use git:
1. Suppose folder 'XD' is to be a local repo then: 
    >> cd XD
    >> git init
    (to check if .git is there) >> ls -a
2. >> git status (for status)
3. to add a file to the repo (file which is present in the folder)
>> git add <file name>
to remove a file from repo
git rm --cached <file>
if >> rm <file> done then it will be removed from local not from repo
if >> git rm -f <file> then removed from both repo and local
4. After any modification to a file in local,
a) >> git add <file>
b) >> git commit -m "<commit name>"
c) >> git push -u origin master (will update the file in remote)
5. >> git log (all commit details can be seen)
6. to clone a repo (from github etc)
>> git clone <copy link for the repo>
Now u need to access via tokens
https://github.com/settings/tokens (to make a token)
then remove previous origin
>> git remote remove origin
>> git remote add origin https://<token>@github.com/GnosGnas/<repo name>.git
Now git remote -v will show this link as the origin
7. 
8. to fix broken commit
>> git commit --amend
