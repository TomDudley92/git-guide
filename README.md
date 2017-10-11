# git-guide

Test repository created for test community meeting

# Merging via terminal: 

Go to the master branch
```git checkout master```

Get the latest version of master
```git pull origin master```

Git gathers any commits from the target branch that do not exist in your current branch and stores them in your local repository.
```git fetch```
   
Merge the target branch into your current branch (master)
```git merge --no-ff origin/<branch-name> --no-commit```

This prevents a fast forward. A fast-forward is when, instead of constructing a merge commit, git just moves your branch pointer to point at the incoming commit. 
```--no-ff```

Prevents the merge commit and allows the user to inspect the code before committing.
```--no-commit```

Once you've reviewed the code and you're happy:
```git commit --author=<author's email address>```

You can type in the first few characters and it will pick up the email address if you've already merged a pr for this person.
For example:
```git commit --author=tes```

That would pick up test.email@digital.hmrc.gov.uk

>>>>>>> Updated readme






