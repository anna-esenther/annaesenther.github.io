# Anna Esenther - Academic Website

Professional academic website for Anna Esenther, Economics PhD student at Harvard University.

## Setup Instructions

### 1. Create GitHub Repository

1. Go to [GitHub](https://github.com/new)
2. Create a new repository named `annaesenther.github.io`
3. Make it public
4. Don't initialize with README (we already have files)

### 2. Push to GitHub

From this directory, run:

```bash
git add .
git commit -m "Initial commit: Professional academic website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/annaesenther.github.io.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

### 3. Enable GitHub Pages

1. Go to your repository settings
2. Navigate to Pages (in the left sidebar)
3. Under "Source", select "Deploy from a branch"
4. Select branch: `main` and folder: `/ (root)`
5. Click Save

### 4. Configure Custom Domain

1. In your repository settings under Pages, enter `annaesenther.com` in the Custom domain field
2. In your domain registrar (where you bought annaesenther.com):
   - Add a CNAME record pointing `www` to `annaesenther.github.io`
   - Add A records for the apex domain (@) pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
3. Wait for DNS propagation (can take up to 24 hours)
4. Check "Enforce HTTPS" in GitHub Pages settings (after DNS is set up)

### 5. Customize Your Website

#### Add Your Profile Photo
- Place a professional headshot at `assets/images/profile.jpg`

#### Update Content
Edit these files with your information:
- `index.md` - Update research interests, contact info
- `cv.md` - Add your education, publications, etc.
- `teaching.md` - Add your teaching experience
- `_config.yml` - Update your email

#### Optional: Add PDF CV
- Place your CV PDF at `assets/cv.pdf` for the download link to work

### 6. Local Testing (Optional)

To preview your site locally:

```bash
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000`

## Customization Tips

- The site uses Harvard crimson colors (#A51C30)
- Modify `assets/css/style.scss` to change styling
- All pages use Markdown for easy editing
- Add new pages by creating `.md` files and adding them to `_config.yml`

## Maintenance

- Update your CV and publications regularly
- Add news/updates to the homepage when you have presentations or papers
- Keep teaching page current with each semester

## Support

For Jekyll documentation: https://jekyllrb.com/docs/
For GitHub Pages help: https://docs.github.com/en/pages
