# Git cheat-sheet

## Create upstream branch on push
```
git push --set-upstream origin featureA
```
What this command will do is, it will set a global configuration that instructs git to push to the current branch and if there’s no upstream branch for the same, it will create one automatically and push henceforth.  
Ref: <https://www.amitmerchant.com/push-newly-branch-without-upstream/>

## Delete all local branches except master
```
git branch | grep -v "master" | xargs git branch -D
```

## Save Credentials
```
git config credential.helper store
```
