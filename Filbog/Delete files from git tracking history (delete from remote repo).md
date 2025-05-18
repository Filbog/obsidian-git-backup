
If we added them via *git add .* :  
```
git rm -r --cached filename
```
then commit and push. That said, if we already committed the files in any previous commit - they'll be somehow still present if we push the to remote repo, even if we have them untracked in the last commit. In that case, we have to **delete the commit/s with which we started tracking them**. This will delete a particular commit:
```bash
git reset --hard <commit-id>
```
If we for example did like 3 commits and are not sure in which commit the files started to be tracked, we can delete those 3 commits with this command (without actually modifying the local files obviously):
```bash
git reset --hard HEAD~3
```
