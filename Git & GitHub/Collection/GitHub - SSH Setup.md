>[!hint] 1 - Check if you already have SSH keys
>Run this in your terminal:
>```bash
>ls -al ~/.ssh
>```
>- If you see files like `id_rsa` and `id_rsa.pub` or `id_ed25519` and `id_ed25519.pub` — you already have keys. If not, create one:

>[!hint] 2 - Generate SSH key
>```bash
>ssh-keygen -t ed25519 -C "your_email@example.com"
>```
>- Use your GitHub email.
>- When it asks for file location, just press Enter to save at default.
>- Optionally set a passphrase for extra security.

>[!hint] 3 - Add your ≥SSH key to the SSH agent
>Start the ssh-agent:
>```bash
>eval "$(ssh-agent -s)"
>```
>Add your key:
>```bash
>ssh-add ~/.ssh/id_ed25519
>```
>>(or `id_rsa` if you generated RSA instead of ed25519)

---
>[!hint] 4 - Add SSH key to GitHub
>Copy your public key:
>```bash
>cat ~/.ssh/id_ed25519.pub
>```
>- Copy the entire output.
>- Go to GitHub ➔ Settings ➔ SSH and GPG Keys ➔ New SSH Key ➔ Paste it.

>[!hint] 5 - Test the SSH connection
>```bash
>ssh -T git@github.com
>```
>If everything is correct, you’ll see something like:
>>Hi `your-username`! You've successfully authenticated...

>[!hint] 6 - Use SSH for your git remotes
>When cloning repos, use SSH link instead of HTTPS:
>```bash
>git clone git@github.com:username/repo.git
>```
>Or change existing remote:
>```bash
>git remote set-url origin git@github.com:username/repo.git
>```

✅ **Done. From now, GitHub won't ask for your credentials when you push/pull.**