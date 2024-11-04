# tower-of-hanoi
Robotics project for solving the Tower of Hanoi problem both algorithmically and with user input.

## Instructions:
Create a directory for the final project in the VM, inside workspaces: 
```
mkdir -p ~/workspaces/final-project
```
Clone repository into ```'~/workspaces/final-project'.```

When modifying code, do it on your branch (not ```main```). To create a branch:
```
git branch <my_branch_name>
git checkout origin/<my_branch_name>
```
Keep your modifications on branch from your local machine updated in the cloud by committing when you make important changes. Make sure you are on your branch when these modifications are made (you can always check with ```git status```.:
```
git add .
git commit -m "<description of commit here>"
git push
```
'.' adds all modified files. You can also specify individual files in place of the '.' to commit specific changes.

Note that only files in the ```'/src'``` folder will be included to prevent issues (ignores changes made to ```'/build'```, ```'/log'```, and ```'/install'```).

When you are ready to merge your branch to the public ```main``` branch, you can make a pull request. Make sure you have pulled all of the previous changes to main onto your local machine:
```
git checkout origin/main
git pull
```
Then, switch to your branch, making sure all of your current changes have either been committed (and pushed if you want to save the version before rebasing) or stashed. Finally, rebase off of main (which has all the updated code from others' commits since you last branched off of it).
```
git checkout <my_branch_name>
git rebase main
```
If there are any merge conflicts (which may occur if the same file was modified on two separate branches), resolve them by keeping the most recent changes. If you want to undo the rebase:
```git rebase --abort```.

Finally, make a pull request on GitHub, with main as the target branch, migrating your changes back into the main branch.

In general, if we all are working on independent files there should (hopefully) be minimal merge conflicts.

