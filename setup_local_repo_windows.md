---
---

# Local Git Repository → GitHub → GitHub Pages Static Site (Windows)

## 0 — What This Does
Creates a local Git repository, links it to GitHub, publishes it as a static website using GitHub Pages, and exposes the site URL in the repository info.

---

## 1 — Tools You Must Have

1. Git  
   https://git-scm.com  
   Install with all default options.

2. Visual Studio Code  
   https://code.visualstudio.com  
   Install with default options.

3. GitHub account  
   https://github.com

---

## 2 — GitHub Authentication
GitHub does not accept passwords for Git operations.

### Create a Personal Access Token (PAT)

1. On GitHub: Profile → Settings
2. Developer settings → Personal access tokens → Tokens (classic)
3. Generate new token
4. Select scope: repo
5. Generate token
6. Copy and store the token securely

When Git asks for a password, paste the token.

> NOTE: You may _not_ be prompted if Git already has your credentials saved. This is normal. This step is something for first time users and it won't hurt to know how to generate a token!

---

## 3 — Create the GitHub Repository

1. Log in to GitHub
2. Click New repository
3. Enter repository name
4. Do NOT check:
   - Add a README
   - Add .gitignore
   - Add a license
5. Click Create repository
6. Copy the HTTPS repository URL (ends in .git)

---

## 4 — Create Local Project Folder and Open in VS Code

1. Create or choose a folder on your computer
2. Open Visual Studio Code
3. File → Open Folder
4. Select the folder
5. View → Terminal

---

## 5 — Initialize Git and Connect to GitHub

In the terminal, enter:

git init  
git remote add origin <paste-repo-URL>  
git remote -v

> Confirm that both fetch and push URLs appear (if you see an error here and don’t know why, the simplest fix is to delete the local folder and repeat steps 4–7. The GitHub repo does not need to be recreated.)

---

## 6 — Create a Basic Static Site

GitHub Pages requires an entry file.

1. In the project folder, create a file named:
   index.html

2. Add minimal content:

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>My Site</title>
</head>
<body>
  <h1>Hello, world</h1>
</body>
</html>

3. Save the file.

---

## 7 — First Commit and Push (Using VS Code Source Control)

1. In VS Code, click **Source Control**  
   (the branching icon: three dots connected by lines)

2. Under **Changes**, click **Stage All**  
   (the **+** icon), or stage individual files

3. In the **Message** field, enter:  
   initial site

4. Click **Commit**

5. Click **Publish Branch**  
   (or **Sync Changes**, if shown)

If prompted:
- Username: your GitHub username
- Password: paste your Personal Access Token (PAT)

If **Publish Branch** does not appear:
1. Press **Ctrl+Shift+P**
2. Run: **Git: Publish Branch**

---

## 8 — Enable GitHub Pages

1. Open the repository on GitHub
2. Go to Settings
3. Select Pages from the left sidebar
4. Under Build and deployment:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: / (root)
5. Click Save

When the Save button is no longer clickable, look to the left column for Pages and click that. Copy the URL of your live site. The Pages site will not appear until at least one successful push to main exists.

---

## 9 — Add the Pages URL to Repository Info

1. Go to the repository main page
2. Click the gear icon next to About
3. Check Website
4. Paste the GitHub Pages URL  
   Example: https://username.github.io/repository-name/
5. Save

This makes the site link visible on the repository page.

---

## 10 — Verify the Site

1. Open the Pages URL in a browser
2. Confirm index.html loads
3. If it does not:
   - Wait 2 minutes
   - Hard refresh (Ctrl+F5)

---

## 11 — Ongoing Workflow

Edit files in VS Code and save changes.

To publish updates:
1. Open Source Control (the icon looks like a circuit diagram)
2. Stage files (+)
3. Enter a commit message
4. Commit
5. Sync Changes

Updates will appear on the site after a short delay.

---

## 12 — Pull Remote Updates (for collaborating with outers or if you sync changes from different computers, etc.)

Either:
- Click Sync Changes
- Or in terminal:

git pull

---

## 13 — Safe Diagnostic Command

At any time, run:

git status

This command never changes files and explains Git’s current state.

---

## 14 — Making Changes

In VS Code, change the text in the index.html page between the <h1> tags to add an exclamation point.

The Source Control icon should show a number, click it. 

In the Message field, write a short description of your change.

Below the Commit button, click the plus sign <+> by the word "Changes" (this "stages" the changes)

Click Commit, then Sync Changes.

If you check your repository, the index.html page should show your changes, they will take time to appear on your website, however. 

Next we will add an extension called "Live Server" so that we don't have to wait for the site to update to see our changes. Well also add extensions to help us with spell checking, HTML coding and Markdown _but this is a good stopping point!  


#### End of instructions.
