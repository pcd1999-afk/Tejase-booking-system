# How to Push to GitHub - Step by Step

## Before You Start
You need:
- A GitHub account (free at github.com)
- Git installed on your device

## Step 1: Create Repository on GitHub
1. Go to github.com and log in
2. Click the "+" icon in top right
3. Click "New repository"
4. Fill in:
   - Repository name: `danielle-booking-system`
   - Description: "Appointment booking system for Danielle"
   - Make it Public or Private (your choice)
   - **IMPORTANT**: Do NOT check "Add a README file"
5. Click "Create repository"

## Step 2: Copy Your Repository URL
After creating, you'll see a page with commands. Look for:
```
https://github.com/YOUR-USERNAME/danielle-booking-system.git
```
Copy this URL!

## Step 3: Open Terminal/Command Prompt
On your device, navigate to where you saved the `danielle-booking-system` folder.

## Step 4: Run These Commands

```bash
# Navigate to the folder
cd danielle-booking-system

# Connect to GitHub (paste YOUR repository URL here)
git remote add origin https://github.com/YOUR-USERNAME/danielle-booking-system.git

# Push your code
git push -u origin main
```

## Step 5: Enter GitHub Credentials
When prompted:
- Username: Your GitHub username
- Password: Your GitHub Personal Access Token (NOT your regular password)

### How to Get a Personal Access Token:
1. GitHub → Settings (your profile) → Developer settings
2. Personal access tokens → Tokens (classic)
3. Generate new token → Give it "repo" permissions
4. Copy the token and use it as your password

## Step 6: Verify
Go to your GitHub repository page and refresh. You should see all your files!

---

## Option 2: GitHub Desktop (Easier for Beginners)

1. Download GitHub Desktop (desktop.github.com)
2. File → Add Local Repository
3. Choose the `danielle-booking-system` folder
4. Click "Publish repository"
5. Choose public/private and click "Publish"

Done! 🎉

---

## Enable GitHub Pages (Optional - For Live Demo)

1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll down to "Pages" (left sidebar)
4. Under "Source":
   - Branch: main
   - Folder: / (root)
5. Click "Save"
6. Wait 2-3 minutes
7. Visit: `https://YOUR-USERNAME.github.io/danielle-booking-system/`

Your booking system is now live on the internet! 🌐

---

## Troubleshooting

### "fatal: not a git repository"
You're not in the right folder. Use `cd` to navigate to `danielle-booking-system`

### "remote origin already exists"
Run: `git remote remove origin` then try again

### "failed to push"
Make sure you created the repository on GitHub first and you're using a Personal Access Token, not your password

### Still stuck?
The folder is already set up with Git. All you need to do is connect it to GitHub and push!
