Assuming:
1. A Github account has been setup already 
2. ssh keys have been setup: `ssh-keygen` copy `id_rsa.pub` to github account
3. git is installed `sudo apt-get install git`

!!! EASIER - ALWAYS CREATE A NEW REPO ON GITHUB FIRST RATHER THAN CONNECTING LOCAL REPO TO GITHUB !!!

# New Repository

1. Go to github and create a new repository.

2. It will give you and option to `ssh` clone the repository - copy this link

3. Go the folder you want to use on your local machine and paste the following:

```
git clone ssh_clone_address
```

4. Try `git remote -v`

5. Make add files

6. Do `git status` do see the changes

7. Do `git add .` to add all changes

8. Do `git commit -m "comment"`

9. Do `git push`

# Existing Repository

Do the following:

0. Create repo in github

1. `git init`

2. `git status`

3. `git add .`

4. Connect to repo:

```
git remote add origin git@github.com:bbdev18/sebowatest.git
```

5. `git commit -m "comment"`

6. Do `git push --set-upstream origin master`

7. `git remote -v`

# Setup .gitignore

You can ignore files and directories:

# all log files will be ignored
logs/
# ignore this file
db.sqlite3
# ignore all files with this type
*.pyc

# Troubleshooting

The following will require a username and password each time:

```
git remote add https://github.com/bbdev18/sebowatest.git
```

1. If it asks for username and password:

check:

The following might not be necessary if you are using ssh properly (check):

```
Check `git config -l` if it has been setup, if not do:

git config --global user.name username
git config --global user.email email@address.com
```

edit `repo_home/.git/config`

```
[remote "origin"]
        url = git@gitlab.com:myaccount/myrepo.git
        # url = https://myaccount@gitlab.com/myaccount/myrepo.git
        fetch = +refs/heads/*:refs/remotes/origin/*
```


