# FastFit GitHub Pages

This directory contains the GitHub Pages site for FastFit Extension, including the Privacy Policy.

## Files

- `index.html` - Landing page for the GitHub Pages site
- `privacy-policy.html` - Privacy Policy page (required for Chrome Web Store submission)

## Setup Instructions

### 1. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - **Source**: Deploy from a branch
   - **Branch**: `main` (or `master`)
   - **Folder**: `/docs`
5. Click **Save**

### 2. Repository URLs

The repository URLs are already configured for:
- Repository: `https://github.com/usesalt/FastFit`
- GitHub Pages: `https://usesalt.github.io/FastFit/`

### 3. Deploy

The GitHub Actions workflow (`.github/workflows/deploy-pages.yml`) will automatically deploy when you:
- Push changes to the `docs/` directory on the `main` branch
- Or manually trigger the workflow from the Actions tab

### 4. Access Your Site

Once deployed, your site will be available at:
```
https://usesalt.github.io/FastFit/
```

The privacy policy will be at:
```
https://usesalt.github.io/FastFit/privacy-policy.html
```

### 5. Use in Chrome Web Store

When submitting to Chrome Web Store, use this URL for the Privacy Policy:
```
https://usesalt.github.io/FastFit/privacy-policy.html
```

## Manual Deployment (Alternative)

If you prefer not to use GitHub Actions:

1. Enable GitHub Pages as described above
2. Simply push your changes to the `docs/` directory
3. GitHub will automatically build and deploy from the `/docs` folder

## Notes

- Changes may take a few minutes to appear after pushing
- The site uses a custom domain if configured, otherwise uses `github.io`
- All files in the `docs/` directory will be publicly accessible

