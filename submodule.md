To get a submodule

```
git submodule update --init --recursive
```

Note, if you make changes to the submodule files or folders and do git status it will show it will not be tracked like
your main local repo. You will need to `cd` into that folder and note that the branch is is `detached` from `head`.

You will need to checkout to the branch you want using `git checkout branchname`. 

Then you can check for changes with `git status` then `git add .` then do `git commit`.

You won't be able to do `git push` remotely you will need to do:

`git push --set-upstream origin branchname`

You will notice now if you go back to your main folder, make some changes to the files in submodule, then do a git status you 
will see the submodule is now being tracked in the branch you chose.
