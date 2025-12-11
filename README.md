# Personal Portfolio Website

A modern, responsive portfolio website featuring Home, About, Contact, and Photos pages.

## Features

- 🏠 **Home Page** - Welcome section with hero content and feature highlights
- 👤 **About Page** - Personal information, skills, and background
- 📧 **Contact Page** - Contact information and message form
- 📸 **Photos Page** - Gallery of projects and photos
- 📱 **Responsive Design** - Works on all devices (desktop, tablet, mobile)
- 🎨 **Modern UI** - Clean and professional design

## How to Push to GitHub and Deploy

### Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com)
2. Sign up for a free account

### Step 2: Create a New Repository on GitHub
1. Log in to GitHub
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Name your repository: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
   - **Important**: This naming format enables GitHub Pages automatically!
   - Example: If your username is `jeramae`, name it `jeramae.github.io`
5. Make it **Public** (required for free GitHub Pages)
6. **Don't** initialize with README, .gitignore, or license (we already have files)
7. Click **"Create repository"**

### Step 3: Initialize Git in Your Project Folder

Open your terminal/command prompt in the project folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Create your first commit
git commit -m "Initial commit: Portfolio website"
```

### Step 4: Connect to GitHub and Push

```bash
# Add your GitHub repository as remote (replace YOUR_USERNAME with your actual username)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Note**: You'll be prompted for your GitHub username and password. For password, you'll need to use a **Personal Access Token** (see Step 5).

### Step 5: Create a Personal Access Token (for authentication)

1. Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Click **"Generate new token (classic)"**
3. Give it a name like "Portfolio Upload"
4. Select scopes: Check **"repo"** (this includes all repo permissions)
5. Click **"Generate token"**
6. **Copy the token immediately** (you won't see it again!)
7. When pushing, use this token as your password

### Step 6: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select **"Deploy from a branch"**
5. Choose branch: **"main"**
6. Choose folder: **"/ (root)"**
7. Click **"Save"**

### Step 7: Access Your Live Website

Your portfolio will be live at:
```
https://YOUR_USERNAME.github.io
```

It may take a few minutes to deploy. You'll see a green checkmark when it's ready!

## Customizing Your Portfolio

### Update Personal Information

1. **Contact Page** (`contact.html`):
   - Update email, phone, location
   - Update LinkedIn and GitHub links

2. **About Page** (`about.html`):
   - Edit the about text
   - Update skills list

3. **Home Page** (`index.html`):
   - Update hero title and subtitle
   - Modify feature cards

### Adding Your Photos

1. Create an `images` folder in your project
2. Add your photos to the `images` folder
3. In `photos.html`, replace the placeholder SVGs with:
   ```html
   <img src="images/your-photo.jpg" alt="Description">
   ```

### Changing Colors

Edit `styles.css` and modify the CSS variables at the top:
```css
:root {
    --primary-color: #6366f1;  /* Change this to your preferred color */
    --secondary-color: #8b5cf6;
    /* ... */
}
```

## File Structure

```
jeramae/
├── index.html      # Home page
├── about.html      # About page
├── contact.html    # Contact page
├── photos.html     # Photos page
├── styles.css      # All styling
├── script.js       # JavaScript functionality
└── README.md       # This file
```

## Future Updates

To update your portfolio after making changes:

```bash
# Add changed files
git add .

# Commit changes
git commit -m "Description of your changes"

# Push to GitHub
git push
```

Your changes will automatically update on GitHub Pages!

## Troubleshooting

### GitHub Pages not showing?
- Wait 5-10 minutes for deployment
- Check Settings → Pages to ensure it's enabled
- Make sure your repository is public
- Verify the repository name matches `username.github.io`

### Can't push to GitHub?
- Make sure you're using a Personal Access Token (not password)
- Verify your remote URL is correct: `git remote -v`
- Check that you have internet connection

### Need Help?
- GitHub Docs: [docs.github.com](https://docs.github.com)
- GitHub Pages Guide: [pages.github.com](https://pages.github.com)

---

**Happy coding! 🚀**

