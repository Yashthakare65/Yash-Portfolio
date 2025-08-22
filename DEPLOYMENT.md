# Quick Deployment Guide

## For GitHub Pages

### Step 1: Push to GitHub
```bash
git add .
git commit -m "Portfolio ready for deployment"
git push origin main
```

### Step 2: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section
4. Under **Source**, select **GitHub Actions**
5. Wait for the workflow to complete (check Actions tab)

### Step 3: Access Your Portfolio
Your portfolio will be available at:
`https://yourusername.github.io/repository-name/`

## Manual Deployment (Alternative)

If you prefer manual deployment:

1. Build the project:
```bash
npm run build
```

2. In GitHub repository settings:
   - Go to **Settings** → **Pages**
   - Select **Deploy from a branch**
   - Choose `gh-pages` branch
   - Select `/ (root)` folder
   - Click **Save**

## Troubleshooting

- **Images not showing**: Make sure images are in `public/images/` folder
- **Build fails**: Check that all dependencies are installed (`npm install`)
- **Page not loading**: Wait a few minutes after deployment, GitHub Pages can take time to update
- **Permission errors**: Make sure GitHub Pages is enabled in repository settings

## Custom Domain (Optional)

To use a custom domain:
1. Add your domain in repository **Settings** → **Pages**
2. Update your DNS settings
3. Wait for DNS propagation (up to 24 hours)
