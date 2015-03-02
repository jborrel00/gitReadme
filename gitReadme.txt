So you want to use github and git to track and store coding projects and other related documents? Great, let’s break down how to do this in the easiest way possible:

1.
first you need to make a github repository, this can be done from the terminal with the following command:

>curl -u ‘USER’ https://api.github.com/user/repos -d ‘{“name”:”REPO”}’

where USER is your github username and REPO is the name of the repository you want to create

now your repo exists at https://github.com/USER/REPO

2.
now you’re working on a specific project, let’s call it test. test  is in your Documents directory (Documents/test). in test you’re making a program called test.py. Make test.py in test and then set up the git in test

>git init
>git add .
>git commit -m ‘First commit’
>git remote add origin https://github.com/USER/REPO #you set this up beforehand (see part 1.)
>git remote -v
>git push origin master

now you’ve sent test.py to your github repository test. to check, go to github and look at your repos.

for subsequent changes, just push new commits to that repo.
