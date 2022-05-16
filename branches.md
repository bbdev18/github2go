# Switch Branches

## Git Checkout

The easiest way to switch branch on Git is to use the `git checkout` command and specify the name of the branch you want to switch to.

If the destination branch does not exist, you have to append the `-b` option, otherwise you won’t be able to switch to that branch.

```
$ git checkout <existing_branch>
```

```
$ git checkout -b <new_branch>
```

As an example, let’s say that you want to switch to the master branch to another branch named “feature” in your repository.

First, make sure that the target branch exists by running the “git branch” command.

```
$ git branch
```

![image](https://user-images.githubusercontent.com/63326895/168520830-c617fd15-ee31-42db-9aec-538bdc2fe3a6.png)

Now that you made sure that your branch exists, you can switch from the master branch to the `feature` branch by executing the `git checkout` command.

```
$ git checkout feature
```

![image](https://user-images.githubusercontent.com/63326895/168520913-1e98eed7-7b07-4804-be66-c29a522ca4b1.png)

## Git Switch

A quick way of switching branch on Git is to use the `git switch` command and specify the name of the branch you want to switch to.

If the destination branch does not exist, you have to specify the `-c` option (for `create branch`), otherwise you will get an error message when switching to that branch.

```
$ git switch <existing_branch>
```

```
$ git switch -c <non_existing_branch>
```

Again, as an example, let’s say that you want to switch to the `feature` branch from the `master` branch.

In order to switch from the `master` branch to the `feature` branch, use the `git switch` command and specify the destination branch (which is `feature` in this case)

```
$ git switch feature
```

![image](https://user-images.githubusercontent.com/63326895/168521324-422cd2d4-356d-417c-ac29-02a2fdeb2cf5.png)


## Checkout New Branch from Specific Commit

https://devconnected.com/how-to-switch-branch-on-git/#Switch_branch_using_git_switch

