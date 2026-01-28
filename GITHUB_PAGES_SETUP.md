# GitHub Pages Setup

This repository is configured to deploy to GitHub Pages automatically.

## How to Enable GitHub Pages

To enable GitHub Pages for this repository, follow these steps:

1. **Go to Repository Settings**
   - Navigate to your repository on GitHub
   - Click on "Settings" in the top menu

2. **Configure GitHub Pages**
   - In the left sidebar, click on "Pages" under "Code and automation"
   - Under "Source", select "GitHub Actions" from the dropdown menu
   - The deployment workflow will now run automatically on pushes to the `main` branch

3. **Verify Deployment**
   - After pushing to the `main` branch, go to the "Actions" tab
   - You should see a workflow run for "Deploy to GitHub Pages"
   - Once complete, your site will be available at: `https://<username>.github.io/<repository-name>/`

## Manual Deployment

You can also trigger a manual deployment:

1. Go to the "Actions" tab in your repository
2. Select "Deploy to GitHub Pages" workflow
3. Click "Run workflow" button
4. Select the branch and click "Run workflow"

## Local Development

To preview the site locally:

1. Open `index.html` in your web browser, or
2. Run a local web server:
   ```bash
   python3 -m http.server 8000
   ```
   Then visit `http://localhost:8000`

## Customization

- Edit `index.html` to customize the content of your GitHub Pages site
- The workflow in `.github/workflows/deploy.yml` will automatically deploy changes when pushed to `main`

## Files

- `.github/workflows/deploy.yml` - GitHub Actions workflow for deployment
- `index.html` - Main page of the website
- `README.md` - Repository documentation
