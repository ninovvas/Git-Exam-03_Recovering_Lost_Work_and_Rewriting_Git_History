# Recovery Demo


## Reflog after --force push

![alt text](images/image.png)

## Adapt the file using rabase -i

![alt text](images/image-1.png)

# Git log
![alt text](images/image-2.png)

## Git reflog

![alt text](images/image-3.png)

## Using commands to solve the task

```bash
git init
echo "# Recovery Demo" > README.md
git add README.md
git commit -m "Initial commit"
echo "Feature A" > featureA.txt
git add .
git commit -m "Add Feature A"
echo "Feature B" > featureB.txt
git add .
git commit -m "Add Feature B"
echo "Fix A" >> featureA.txt
git add .
git commit -m "Fix bug in Feature A"
git reflog
git checkout -b outdated HEAD~2
git checkout master
git remote add origin https://github.com/ninovvas/Git-Exam-03_Recovering_Lost_Work_and_Rewriting_Git_History.git
git push -u origin master
git status
git reset --hard HEAD~2
git push origin master --force
git reflog
git reset --hard 5695778
git reflog
git rebase -i HEAD@{7}
git rebase --continue
git reflog
git push origin master --force-with-lease
git status
git log --oneline
git reflog
git status
git add .
git commit -m"Add documentation to README.md file"
```
