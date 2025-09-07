# Deploying Lyell_Website to Vercel (Free Tier)

Follow these steps to deploy your static website to [Vercel](https://vercel.com):

---

## 1. Sign Up / Log In to Vercel

- Visit [vercel.com](https://vercel.com).
- Sign up or log in (GitHub, GitLab, Bitbucket, or email).

---

## 2. (Optional) Install Vercel CLI

- Open your terminal.
- Run:
  ```
  npm install -g vercel
  ```

---

## 3. Prepare Your Project

- Ensure all website files are in a folder (e.g., `/Users/Santu/LEARNING/Lyell_Website`).
- The main entry file should be `index.html`.

---

## 4. Push Your Project to GitHub (Recommended)

- Initialize a git repository:
  ```
  cd /Users/Santu/LEARNING/Lyell_Website
  git init
  git add .
  git commit -m "Initial commit"
  ```
- Create a new repository on GitHub.
- Add the remote and push:
  ```
  git remote add origin https://github.com/yourusername/your-repo-name.git
  git push -u origin master
  ```

---

## 5. Import Project to Vercel

- In the Vercel dashboard, click **"Add New Project"**.
- Select your GitHub repository.
- Vercel auto-detects static sites.

---

## 6. Configure Build Settings

- For static sites:
  - **Framework Preset:** Other
  - **Build Command:** (leave blank)
  - **Output Directory:** (leave blank or set to `.`)

---

## 7. Deploy

- Click **"Deploy"**.
- Wait for deployment to finish.
- You’ll get a live URL (e.g., `https://your-project.vercel.app`).

---

## 8. Direct Upload (Without Git)

- Use Vercel CLI:
  ```
  cd /Users/Santu/LEARNING/Lyell_Website
  vercel
  ```
- Answer the prompts (project name, root directory, etc.).
- Your site will be deployed and you’ll get a URL.

---

## Notes

- **Private Repos:** Your deployed website is public even if your GitHub repo is private. Only your source code remains private.
- You can redeploy by pushing changes to GitHub or running `vercel` in your project folder.