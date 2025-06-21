```bash
echo ".DS_Store" >> .gitignore
git rm --cached .DS_Store
git commit -m "Remove .DS_Store and add to .gitignore"
```