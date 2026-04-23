# Publishing to GitHub - Step by Step

These are one-time setup steps to get the guide onto GitHub with a live URL.

## 1. Create the repo on GitHub

1. Go to https://github.com/new
2. Repository name: `dckc-course-guide`
3. Description: "Guide for DCKC members on organising training courses and assessments"
4. Choose **Public** (needed for free GitHub Pages) or **Private** (if you prefer - Pages still works on private repos with a paid plan, or if the club already has one)
5. Do NOT tick "Add a README" - we already have one
6. Click **Create repository**

## 2. Push the files

Open Terminal, navigate to the folder containing these files (wherever you downloaded them), and run:

```bash
cd path/to/dckc-course-guide-repo

git init
git add .
git commit -m "Initial commit: course organising guide"
git branch -M main
git remote add origin https://github.com/whistule/dckc-course-guide.git
git push -u origin main
```

If prompted for credentials, use a GitHub personal access token (not your password) - see https://github.com/settings/tokens if you don't have one set up.

## 3. Enable GitHub Pages

1. On the repo page, click **Settings** (top right)
2. In the left sidebar, click **Pages**
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: **main** / **/ (root)**
4. Click **Save**
5. Wait 1-2 minutes

Your guide will be live at: **https://whistule.github.io/dckc-course-guide/**

## 4. Link it from dckc.co.uk

Once the GitHub Pages URL is working, add a link to it from the relevant spot on the club website - probably under the "Coaching / Leading" menu since that's where the related PSL pages live.

## 5. Add collaborators

To let the coaching coordinator or committee members edit the guide:

1. Settings → Collaborators
2. Click **Add people** and search by their GitHub username

They'll get an invite email. Once accepted, they can edit `index.html` directly on github.com via the pencil icon.

## Making changes later

Smallest path - edit directly on github.com:

1. Go to the repo
2. Click `index.html`
3. Click the pencil icon (top right)
4. Edit
5. Scroll down, write a short commit message, click **Commit changes**

GitHub Pages will republish automatically within a minute or two.
