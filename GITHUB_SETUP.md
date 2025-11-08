# GitHub Setup Instructions

Your local Git repository is ready! Follow these steps to push it to GitHub:

## Step 1: Create a New Repository on GitHub

1. Go to [GitHub.com](https://github.com) and sign in to your account
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Fill in the repository details:
   - **Repository name**: `filipino-flavors` (or any name you prefer)
   - **Description**: "A modern Filipino food blog website built with HTML and CSS"
   - **Visibility**: Choose Public or Private
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
5. Click **"Create repository"**

## Step 2: Push Your Code to GitHub

After creating the repository, GitHub will show you commands. Use these commands in your terminal:

### Option A: If you haven't set the remote yet (First time)

```bash
cd "C:\Users\User\Downloads\Harold Project"
git remote add origin https://github.com/YOUR_USERNAME/filipino-flavors.git
git branch -M main
git push -u origin main
```

**Replace `YOUR_USERNAME`** with your actual GitHub username.

### Option B: If you need to authenticate

If you're using HTTPS and GitHub asks for authentication:

- You may need to use a **Personal Access Token** instead of your password
- Or use **GitHub CLI** (`gh auth login`)
- Or set up **SSH keys** for authentication

## Step 3: Verify

After pushing, refresh your GitHub repository page. You should see all your files there!

## Troubleshooting

### If you get authentication errors:

1. Use GitHub Personal Access Token:
   - Go to GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)
   - Generate a new token with `repo` permissions
   - Use this token as your password when pushing

### If you need to change the remote URL:

```bash
git remote set-url origin https://github.com/YOUR_USERNAME/filipino-flavors.git
```

### If you want to use SSH instead:

```bash
git remote set-url origin git@github.com:YOUR_USERNAME/filipino-flavors.git
```

## Next Steps

After pushing to GitHub, you can:

- Enable GitHub Pages to host your website
- Add collaborators
- Create issues and pull requests
- Continue developing and pushing updates

---

**Your local repository is ready to push!** 🚀
