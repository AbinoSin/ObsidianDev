>[!done] ✅ **Collaborative branch-based workflow with restricted permissions**

>[!faq] Goal?
>**Your *friend* can:**
>- Clone
>- Work on a separate branch
>- Push changes to that branch
>
>**Only *you* can**:
>- Merge into `main` (or `master`)

---
### 1️⃣ Add your friend as a **Collaborator**
- Go to your GitHub repo → **_Settings_ → _Collaborators_ and _Teams_ → Add _collaborator_**
- Enter your friend’s GitHub username → Invite.

>Now your friend can clone and push.

---
### 2️⃣ **Create a branch for your friend**
Either you create branch, or they can create it.
Example (you create it):
```bash
git checkout -b feature-friend
git push origin feature-friend
```
>Now branch `feature-friend` exists.

---
### 3️⃣ **Set Branch Protection Rules (important part)**
- Go to your GitHub repo → ***Settings* → *Branches* → *Branch Protection Rules***
- Select your main branch (e.g. `main`)

👉 **Enable**:
- ✅ Require pull request before merging
- ✅ Require approvals (optional if you work alone)
- ✅ Disable force push
- ✅ Allow only administrators to push (or limit who can push directly)

>⚠️ This ensures **only you** can directly push/merge into `main`.

---
### 4️⃣ **Workflow:**
**Your *friend***:
- Clones repo.
- Checks out `feature-friend`.
- Works and pushes only to `feature-friend`.

***You***:
- Review his branch.
- Merge via Pull Request (PR) when you approve.

>[!hint] 🚀 Why is this very professional?
>- ✅ Safe  
>- ✅ Full control  
>- ✅ Clean project history  
>- ✅ Good practice for real-world development.