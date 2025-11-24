# GitHub Pages Setup Guide for FastFit

This guide will help you set up GitHub Pages to host the Privacy Policy for your Chrome Web Store submission.

## What Was Created

1. **`docs/privacy-policy.html`** - Your privacy policy page
2. **`docs/index.html`** - Landing page for your GitHub Pages site
3. **`.github/workflows/deploy-pages.yml`** - Automatic deployment workflow

## Step-by-Step Setup

### Step 1: Enable GitHub Pages

1. Go to your GitHub repository: `https://github.com/usesalt/fastfit-pages`
2. Click on the **Settings** tab (top menu)
3. In the left sidebar, scroll down and click **Pages**
4. Under **Source**, configure:
   - **Source**: Select "Deploy from a branch"
   - **Branch**: Select `main` (or `master` if that's your default branch)
   - **Folder**: Select `/docs`
5. Click **Save**

### Step 2: Commit and Push

If you haven't already, commit and push the new files:

```bash
git add docs/
git add .github/workflows/deploy-pages.yml
git commit -m "Add GitHub Pages site with privacy policy"
git push origin main
```

### Step 3: Wait for Deployment

- GitHub Pages will automatically build and deploy your site
- This usually takes 1-2 minutes
- You can check the deployment status in the **Actions** tab of your repository

### Step 4: Access Your Site

Once deployed, your site will be available at:
```
https://usesalt.github.io/FastFit/
```

Your privacy policy will be at:
```
https://usesalt.github.io/FastFit/privacy-policy.html
```

### Step 5: Use in Chrome Web Store

When filling out the Chrome Web Store Privacy Policy form, use:
```
https://usesalt.github.io/FastFit/privacy-policy.html
```

## Verification

1. Visit `https://usesalt.github.io/FastFit/privacy-policy.html` in your browser
2. Verify the page loads correctly
3. Check that all links work
4. Review the content to ensure it's accurate

## Updating the Privacy Policy

To update the privacy policy:

1. Edit `docs/privacy-policy.html`
2. Update the "Last Updated" date at the top
3. Commit and push:
   ```bash
   git add docs/privacy-policy.html
   git commit -m "Update privacy policy"
   git push origin main
   ```
4. Changes will be automatically deployed within 1-2 minutes

## Troubleshooting

### Site Not Loading

- Check the **Actions** tab for any deployment errors
- Verify the branch and folder settings in Pages settings
- Ensure the `docs/` folder is in the root of your repository

### 404 Error

- Make sure the file is named exactly `privacy-policy.html` (case-sensitive)
- Verify the file is in the `docs/` directory
- Check that GitHub Pages is configured to use the `/docs` folder

### Changes Not Appearing

- Wait 1-2 minutes for GitHub to rebuild
- Clear your browser cache
- Check the Actions tab to see if deployment completed successfully

## Custom Domain (Optional)

If you want to use a custom domain:

1. Add a `CNAME` file in the `docs/` directory with your domain
2. Configure DNS settings with your domain provider
3. Update the domain in GitHub Pages settings

## Notes

- The site is publicly accessible once deployed
- All files in `docs/` will be served as static files
- GitHub Pages supports HTTPS by default
- The site will automatically update when you push changes to the `docs/` directory

