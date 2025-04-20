# GitHub Pages Deployment Guide

This guide will walk you through the process of deploying your portfolio website to GitHub Pages, making it accessible online at `yourusername.github.io`.

## Prerequisites

1. A GitHub account - If you don't have one, sign up at [github.com](https://github.com)
2. Git installed on your computer - Download from [git-scm.com](https://git-scm.com/downloads)

## Step-by-Step Deployment Instructions

### 1. Create a GitHub Repository

1. Log in to your GitHub account
2. Click on the "+" icon in the top-right corner and select "New repository"
3. Name your repository exactly as: `yourusername.github.io` (replace "yourusername" with your actual GitHub username)
4. Make sure the repository is set to "Public"
5. Click "Create repository"

### 2. Set Up Git on Your Computer

Open a terminal or command prompt and run the following commands:

```bash
# Configure Git with your identity
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### 3. Clone the Repository

```bash
# Navigate to where you want to store your project
cd /path/to/your/projects

# Clone the empty repository
git clone https://github.com/yourusername/yourusername.github.io.git

# Navigate into the repository folder
cd yourusername.github.io
```

### 4. Copy Your Website Files

Copy all the files from the portfolio website I created for you into this repository folder:

```bash
# Copy all files from the portfolio folder to your repository folder
# Replace /path/to/ammar-portfolio with the actual path to your portfolio files
cp -r /path/to/ammar-portfolio/* /path/to/yourusername.github.io/
```

### 5. Commit and Push Your Website

```bash
# Add all files to Git
git add .

# Commit the files
git commit -m "Initial website deployment"

# Push to GitHub
git push -u origin main
```

Note: If your default branch is called "master" instead of "main", use `git push -u origin master` instead.

### 6. Verify Deployment

1. Go to your GitHub repository at `https://github.com/yourusername/yourusername.github.io`
2. Navigate to Settings > Pages
3. You should see a message saying "Your site is published at https://yourusername.github.io"
4. It may take a few minutes for your site to be published
5. Visit `https://yourusername.github.io` to see your live website

## Making Updates to Your Website

Whenever you want to update your website, follow these steps:

1. Make changes to your local files
2. Add the changes: `git add .`
3. Commit the changes: `git commit -m "Description of changes"`
4. Push to GitHub: `git push`
5. Wait a few minutes for GitHub Pages to update

## Using a Custom Domain (Optional)

If you have your own domain name, you can use it with GitHub Pages:

1. Go to your repository settings
2. Scroll down to the "GitHub Pages" section
3. Under "Custom domain", enter your domain name (e.g., `www.yourname.com`)
4. Click "Save"
5. Create a CNAME record with your domain registrar pointing to `yourusername.github.io`

## Troubleshooting

- If your site isn't published, check the "GitHub Pages" section in your repository settings
- Ensure your repository is named exactly `yourusername.github.io`
- Make sure your repository is public
- Check that your files are in the root of the repository, not in a subfolder

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Setting up a custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [GitHub Guides](https://guides.github.com/)
