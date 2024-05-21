# Part 1

### Exercise 1 - 7

```bash
  381  touch test{1..4}.md
  382  git add test1.md && git commit -m "chore: Create initial file"~
  383  git add test1.md && git commit -m "chore: Create initial file"
  384  git add test2.md && git commit -m "chore: Create another file"
  385  git add test3.md && git commit -m "chore: Create third and fourth files"
  386  git status
  387  git log
  388  git add test4.md
  389  git commit --ammend -m "Added third and fourth file"
  390  git commit --amend -m "Chore: Added third and fourth file"


  391  git rebase -i HEAD~2
  392  git rebase -i HEAD~2
  393  git commit --amend
  394  git rebase -i HEAD~3
  395  cls
  396  git log
  397  git rebase -i HEAD~2
  398  git rebase --continue
  399  git log
  400  git rebase -i HEAD~2
  401  git rebase -i
  402  git rebase -i HEAD~2
  403  git rebase -i --root


  404  git status
  405  git reset HEAD~
  406  git status
  407  git add test3.md
  408  git commit -m "Create Third File"
  409  git add test4.md
  410  git commit -m "Create Fourth file"


  411  git log
  412  git rebase -i HEAD~2
  413  git rebase -i --root
  414  touch unwanted.txt
  415  git add unwanted.txt
  416  git commit -m "Unwanted commit"
  421  git rebase -i --root
  422  git log
  423  git rebase -i -root
  425  git rebase -i -root
  426  git rebase -i --root
  427  git log


```

### Exercise 8

```bash

  432  git checkout -b ft/branch
  433  touch test5.md
  434  git add test5.md
  435  git commit -m "Implemented test 5"
  436  git checkout main
  437  git cherry-pick ft/branch
  
```

### Exercise 9 - 10

```bash
  439  git log --graph --oneline --all
  440  git reflog
```

# Part 2

### Exercise 1 - 5

```bash
  448  git checkout -b ft/new-feature
  449  touch feature.txt
  450  git add feature.txt
  451  git status
  452  git status
  453  git add .
  454  git status
  455  git commit -m "Implemented core functionality for new feature"
  456  git checkout main
  457  touch readme.txt
  458  git status
  459  git add readme.txt
  460  git commit -m "Updated project readme"
  461  git push
  462  git checkout -d ft/new-feature

```

### Exercise 6 - 10

```bash
  465  git log
  466  git log --oneline
  467  git checkout -b ft/new-branch-from-commit 4c1dfe7
  468  git checkout main
  469  git merge ft/new-branch-from-commit
  470  git checkout ft/new-branch-from-commit
  471  git rebase main
  472  git status
  473  git add .
  474  git status
  475  git rebase main
  476  git commit -m "Update README"
  477  git rebase main
  478  git branch -m ft/new-branch-from-commit ft/improved-branch-name
  479  git log --oneline
  480  git checkout 7dc5ea1

```

# Part 3

### Exercise 1 - 3

```bash

  495  git stash
  496  git stash pop
  497  touch conflict.txt
  498  git add conflict.txt
  499  git commit -m "Add conflict file in main"
  500  git checkout -b ft/conflict
  501  touch conflict.txt
  502  git add conflict.txt
  503  git commit -m "Add conflict file in confict file"
  504  git checkout main
  505  git merge ft/conflict
  506  git add conflict.txt
  507  git merge ft/conflict
  508  git status
  509  git add conflict.txt
  510  git status
  511  git checkout ft/conflict
  512  checkout main
  513  git checkout main
  514  git add .
  515  git status
  516  git commit -m "Create conflict on main"
  517  git checkout ft/conflict
  518  git status
  519  git add .
  520  git status
  521  git commit -m "Create conflict on ft branch"
  522  git checkout main
  523  git merge ft/conflict
  524  git add .
  526  git commit -m "Resolved conflict"

```

### Exercise 4 

```bash


```