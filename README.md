# carlopach-website
Static site for Carlo Pach art

## Overview
This is a static HTML/CSS website for Carlo Pach's art portfolio, designed for deployment on GitHub Pages with a custom domain (carlopach.com).

## Features
- **Responsive Design**: Mobile-friendly layout that adapts to different screen sizes
- **Modern UI**: Clean design with gradient accents and smooth animations
- **Portfolio Gallery**: Grid layout to showcase artwork
- **Contact Section**: Easy way for visitors to get in touch
- **Custom Domain**: Configured for carlopach.com

## File Structure
```
.
├── index.html              # Main HTML page
├── styles.css              # CSS styling
├── CNAME                   # Custom domain configuration
├── .github/
│   └── workflows/
│       └── static.yml      # GitHub Actions deployment workflow
└── README.md               # This file
```

## Local Development
To view the site locally:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js
npx http-server

# Then open http://localhost:8000 in your browser
```

## Deployment
The site automatically deploys to GitHub Pages when changes are pushed to the `main` branch via GitHub Actions.

### Setup Instructions:

1. **Enable GitHub Pages**:
   - Go to repository Settings > Pages
   - Source: GitHub Actions

2. **Configure Custom Domain**:
   - The CNAME file is already configured with `carlopach.com`
   - At your domain registrar, add DNS records:
     - **Option A**: Add A records pointing to:
       - 185.199.108.153
       - 185.199.109.153
       - 185.199.110.153
       - 185.199.111.153
     - **Option B**: Add CNAME record pointing to `carlpach.github.io`

3. **Verify Domain**:
   - In repository Settings > Pages, verify your custom domain
   - Enable "Enforce HTTPS" once DNS propagates

## Customization
To customize the site content:
- Edit `index.html` to change text, sections, or structure
- Modify `styles.css` to adjust colors, fonts, or layout
- Replace placeholder artwork sections with actual images

## License
© 2024 Carlo Pach. All rights reserved.
