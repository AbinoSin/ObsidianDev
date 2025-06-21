## Stage
```bash
git add --all         # stage everything
git add .             # stage only current directory

git add filename.html # stage specific file
```
---
## Commit
```bash
git commit -m "Commit Message"
```

>[!cite] Tone of Commit messages
>- Present tense & Imperative.
>- Give instructions to code (don't care 😠).
>```bash
>❌ git commit -m "added footer to the code base"
>✅ git commit -m "add footer"
>```

>[!info] Atomic Commits
>Atomic commits are a way to make sure that each commit is a self-contained unit of work. This means that if one commit fails, you can always go back to a previous commit and fix the issue. This is important for maintaining a clean and organized history in your repository.
>- Keep commits centric to one feature, one component, or on fix.
>- Focused on one thing.