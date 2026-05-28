# Life Tracker — GitHub Setup Guide

This guide gets your app hosted on GitHub Pages and your data syncing to GitHub in about 10 minutes.

---

## Part 1 — Create a GitHub account

1. Go to [github.com](https://github.com) and sign up for a free account
2. Verify your email

---

## Part 2 — Create a repository

1. Click the **+** icon (top right) → **New repository**
2. Name it `life-tracker` (or anything you like)
3. Set it to **Private** (recommended — keeps your personal data private)
4. Check **"Add a README file"** — this initialises the repo
5. Click **Create repository**

---

## Part 3 — Host the app on GitHub Pages

1. In your new repo, click **Add file** → **Upload files**
2. Drag `index.html` into the upload area → click **Commit changes**
3. Go to **Settings** (top menu of the repo) → **Pages** (left sidebar)
4. Under **Source**, select **Deploy from a branch**
5. Set branch to `main`, folder to `/ (root)` → click **Save**
6. Wait ~60 seconds, then your app is live at:
   `https://YOUR-USERNAME.github.io/life-tracker`

> Tip: bookmark this URL and use it to add the app to your phone home screen.

---

## Part 4 — Create a Personal Access Token

This lets the app read and write your data to the repo.

1. Click your **profile photo** (top right) → **Settings**
2. Scroll to the bottom of the left sidebar → **Developer settings**
3. **Personal access tokens** → **Tokens (classic)**
4. Click **Generate new token** → **Generate new token (classic)**
5. Give it a name like `Life Tracker`
6. Set expiration to **No expiration** (or a long period)
7. Under **Select scopes**, tick **repo** (the first checkbox — this covers all repo permissions)
8. Click **Generate token**
9. **Copy the token immediately** — you won't see it again

---

## Part 5 — Connect the app to GitHub

1. Open your app at the GitHub Pages URL
2. Unlock with your PIN → go to **Settings** (bottom nav)
3. Scroll to **GitHub sync**
4. Fill in:
   - **GitHub username** — your GitHub username
   - **Repository name** — `life-tracker` (or whatever you named it)
   - **Personal access token** — paste the token from Part 4
5. Tap **Test connection** — you should see "Connected ✓"
6. Tap **Sync now** — your data is now backed up to GitHub

From this point on, every goal, check-in, and change automatically syncs to GitHub in the background. Your data is safe even if you clear your browser cache.

---

## Accessing your data

Your data lives at:
`https://github.com/YOUR-USERNAME/life-tracker/blob/main/data.json`

You can view it, download it, or even edit it directly in GitHub if needed.

---

## Using on a new device

1. Open the GitHub Pages URL on your new device
2. Go to Settings → fill in the same GitHub credentials
3. Tap **Sync now** — all your goals and history will load

---

## Updating the app

When a new version of `index.html` is available:
1. Go to your repo on GitHub
2. Click `index.html` → click the pencil/edit icon (or upload the new file)
3. GitHub Pages updates automatically within ~60 seconds
