# Troubleshooting Guide

## Common Issues and Solutions

### 1. Permission Denied Error (403)

**Error**: `remote: Permission to Yashthakare65/Yash-Portfolio.git denied to github-actions[bot]`

**Solution**: 
- The new workflow uses the official GitHub Pages action with proper permissions
- Make sure GitHub Pages is enabled in your repository settings
- Go to **Settings** → **Pages** → **Source** → Select **GitHub Actions**

### 2. Images Not Loading

**Problem**: Project images show as broken or don't appear

**Solutions**:
- Check that images are in the `public/images/` folder
- Verify image paths in `src/components/Projects.jsx` use `./images/` format
- Images will show fallback placeholders if they fail to load

### 3. Build Fails

**Problem**: `npm run build` command fails

**Solutions**:
- Run `npm install` to ensure all dependencies are installed
- Check for syntax errors in your React components
- Verify all import statements are correct

### 4. GitHub Pages Not Updating

**Problem**: Changes pushed but website not updated

**Solutions**:
- Check the **Actions** tab in your repository for workflow status
- Wait 5-10 minutes for GitHub Pages to update
- Verify the workflow completed successfully
- Check repository **Settings** → **Pages** for deployment status

### 5. 404 Error on GitHub Pages

**Problem**: Website shows 404 error

**Solutions**:
- Ensure the repository name matches exactly in the URL
- Check that GitHub Pages is enabled and configured correctly
- Verify the workflow deployed to the correct branch

## Workflow Status Check

1. Go to your repository on GitHub
2. Click the **Actions** tab
3. Look for the latest workflow run
4. Check if it shows ✅ (success) or ❌ (failure)
5. Click on the workflow to see detailed logs

## Manual Verification

To verify your build locally:

```bash
# Build the project
npm run build

# Preview the build
npm run preview

# Open http://localhost:5174 in your browser
```

## Still Having Issues?

1. Check the GitHub Actions logs for specific error messages
2. Verify your repository has GitHub Pages enabled
3. Ensure you're pushing to the `main` branch
4. Check that all files are committed and pushed

## Contact Support

If you continue to have issues:
- Open an issue on your repository
- Include the error message and workflow logs
- Describe what you've tried so far
