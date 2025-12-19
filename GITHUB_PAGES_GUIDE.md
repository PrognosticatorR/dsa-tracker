# How to Deploy Your Live DSA Tracker on GitHub Pages

This guide will help you host your `DSA.html` file as a live website so you can access it from anywhere and track your interview preparation progress.

## Prerequisites
- A GitHub account.
- `git` installed on your machine.
- Your `DSA.html` file ready.

## Steps

### 1. Initialize a Git Repository
If you haven't already, turn your `neetcode` folder into a git repository.
Open your terminal in the directory where `DSA.html` is located:

```sh
cd /Users/devesrawat/Desktop/practice/neetcode
git init
```

### 2. Rename the file (Optional but Recommended)
GitHub Pages defaults to serving `index.html`. It's easier if you rename `DSA.html` to `index.html`.
*If you prefer to keep it as `DSA.html`, your live URL will just have `/DSA.html` at the end.*

```sh
# Optional
mv DSA.html index.html
```

### 3. Commit Your Files
Add your files to the repository.

```sh
git add .
git commit -m "Initial commit of DSA Tracker"
```

### 4. Create a Repository on GitHub
1. Go to [GitHub.com](https://github.com) and log in.
2. Click the **+** icon in the top right and select **New repository**.
3. Name it something like `dsa-tracker`.
4. Make it **Public** (GitHub Pages is free for public repos).
5. Click **Create repository**.

### 5. Push to GitHub
Follow the instructions shown on GitHub to push your local code. It will look something like this (replace `YOUR_USERNAME` with your actual username):

```sh
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/dsa-tracker.git
git push -u origin main
```

### 6. Enable GitHub Pages
1. Go to your repository on GitHub.
2. Click on **Settings** > **Pages** (in the left sidebar).
3. Under **Build and deployment**, select **Source** as `Deploy from a branch`.
4. Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
5. Click **Save**.

### 7. Access Your Site
Wait a minute or two. GitHub will provide you with a URL (usually `https://YOUR_USERNAME.github.io/dsa-tracker/`).
- If you renamed the file to `index.html`, just click the link.
- If you kept `DSA.html`, add `/DSA.html` to the end of the URL.

**🎉 You now have a live DSA tracking tool!**
Your progress is saved in your browser's local storage, so it will persist as long as you don't clear your browser data.
