# GitHub Pages Setup Instructions

Follow these steps to connect your portfolio to GitHub and enable automatic deployment with GitHub Pages:

## Step 1: Create a Repository on GitHub

1. Log in to your GitHub account at [github.com](https://github.com)
2. Click the "+" icon in the top right corner and select "New repository"
3. Name your repository: `sarthakahlawat-portfolio`
4. Make sure it's set to "Public"
5. Do not initialize the repository with README, .gitignore, or license (we already have these)
6. Click "Create repository"

## Step 2: Connect Your Local Repository to GitHub

GitHub will show commands to push an existing repository. Copy and run these commands in your terminal:

```bash
git remote add origin https://github.com/sarthakahlawat/sarthakahlawat-portfolio.git
git branch -M main
git push -u origin main
```

Replace `sarthakahlawat` with your actual GitHub username.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" (tab near the top right)
3. Scroll down to the "GitHub Pages" section (or click "Pages" in the left sidebar)
4. Under "Source," select "Deploy from a branch"
5. In the "Branch" dropdown, select "main"
6. In the folder dropdown, select "/ (root)"
7. Click "Save"

## Step 4: Wait for Deployment

GitHub will now start building and deploying your site. This usually takes a minute or two.

## Step 5: Access Your Live Site

Your site will be available at:
```
https://[your-username].github.io/sarthakahlawat-portfolio/
```

For example: `https://sarthakahlawat.github.io/sarthakahlawat-portfolio/`

## Making Changes and Updating the Site

Whenever you want to update your portfolio:

1. Make changes to your files locally
2. Test changes locally using a web server (e.g., `python -m http.server 8000`)
3. Commit your changes:
   ```bash
   git add .
   git commit -m "Description of your changes"
   ```
4. Push to GitHub:
   ```bash
   git push origin main
   ```
5. GitHub Pages will automatically rebuild and deploy your updated site

## Troubleshooting

- **Site not updating?** Check the "Actions" tab in your GitHub repository to see if there are any build errors.
- **404 errors?** Make sure all your file paths are correct and use relative paths.
- **Custom domain?** You can add a custom domain in the GitHub Pages settings.

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/) 