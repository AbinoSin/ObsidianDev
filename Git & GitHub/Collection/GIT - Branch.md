>[!example] List all branches and check current
>```bash
>git branch
>```

>[!example] Manage branches
>```bash
>git branch <branch-name>    # to create branch
>git branch -d <branch-name> # to delete branch
>```
>```bash
># rename branch
>git branch -m <old-branch-name> <new-branch-name>
>```
>```bash
>git switch <branch-name>    # to switch current branch
>git switch -c <branch-name> # to switch (create if not any)
>```

>[!example] Marge branches
>```bash
>git switch <branch-name> # first goto the branch where you want to merge
>git merge <branch-name>  # than merge that branch which you want to merge
>```
>```bash
>git merge --abort # if don't want to merge
>```


