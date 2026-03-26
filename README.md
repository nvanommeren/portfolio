# Portfolio Website

A clean, editorial-style portfolio website for showcasing coding projects.

## Project Structure

```
portfolio/
├── index.html              # Main landing page
├── styles.css              # Global stylesheet
├── script.js               # Animations & interactions
├── projects/               # Individual project pages
│   ├── project-template.html   # Copy this for new projects
│   ├── project-1.html          (create as needed)
│   └── ...
└── assets/                 # Images & media (create as needed)
    ├── images/
    └── screenshots/
```

## Quick Start

1. **Local Development**
   Simply open `index.html` in your browser, or use a local server:
   ```bash
   # Python
   python -m http.server 8000
   
   # Node.js (with npx)
   npx serve .
   
   # VS Code: Use the "Live Server" extension
   ```

2. **View at** `http://localhost:8000`

## Customization

### Update Personal Info
- Edit `index.html`:
  - Hero section: title, subtitle, tagline
  - About section: bio, skills
  - Contact section: email, social links
  - Footer: copyright text

### Add New Projects
1. Copy `projects/project-template.html` as a starting point
2. Rename to match your project (e.g., `my-awesome-app.html`)
3. Update the content (title, description, tech stack, etc.)
4. Add a card in `index.html` under `.projects-grid`
5. Link to your new project page

### Change Colors
Edit CSS variables in `styles.css`:
```css
:root {
    --color-bg: #FAF9F7;          /* Background */
    --color-text: #1A1A1A;        /* Primary text */
    --color-accent: #C45D3A;      /* Accent color (terracotta) */
    --color-text-muted: #6B6B6B;  /* Secondary text */
}
```

### Change Fonts
The site uses Google Fonts:
- **Instrument Serif** - Headlines (elegant, editorial)
- **DM Sans** - Body text (clean, modern)

To change fonts:
1. Pick fonts from [Google Fonts](https://fonts.google.com)
2. Update the `<link>` tag in HTML files
3. Update `--font-display` and `--font-body` in CSS

## Deployment Options

### GitHub Pages (Free)
1. Push to a GitHub repository
2. Go to Settings → Pages
3. Select "Deploy from a branch" → main branch
4. Your site will be at `yourusername.github.io/repository-name`

### Netlify (Free)
1. Drag & drop the `portfolio` folder to [Netlify Drop](https://app.netlify.com/drop)
2. Or connect your GitHub repo for automatic deploys

### Vercel (Free)
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the portfolio directory
3. Follow the prompts

### Custom Domain
After deploying, add a custom domain through your hosting provider's settings.

## Adding Screenshots

1. Create an `assets/screenshots` folder
2. Add project screenshots (recommended: 1600×900px, PNG or WebP)
3. Replace the placeholder divs in project pages:
   ```html
   <!-- Before -->
   <div class="project-image-full">
       <span>Screenshot or Demo GIF</span>
   </div>
   
   <!-- After -->
   <img src="../assets/screenshots/my-project.png" 
        alt="Project screenshot" 
        class="project-image-full">
   ```

## Browser Support

- Chrome, Firefox, Safari, Edge (latest 2 versions)
- Mobile responsive design included

## License

Feel free to use this template for your own portfolio!
