# Portfolio Website

A modern, minimalist portfolio website for showcasing data science projects and applications.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern Aesthetics**: Clean, editorial-inspired dark theme with bold typography
- **Project Showcase**: Dedicated pages for displaying Streamlit apps, Shiny applications, and data visualizations
- **Filtering**: Interactive project filtering by category
- **Smooth Animations**: Subtle scroll-based animations and transitions
- **Easy Customization**: Simple HTML/CSS structure for quick modifications

## Structure

```
portfolio/
├── index.html              # Landing page with About Me section
├── projects.html           # Grid view of all projects
├── css/
│   └── style.css          # Main stylesheet
├── js/
│   └── main.js            # JavaScript for interactivity
├── projects/
│   └── project-template.html  # Template for individual project pages
└── README.md              # This file
```

## Customization Guide

### 1. Update Your Information

**index.html:**
- Replace "Your Name" with your actual name
- Update the hero subtitle
- Modify the About Me text
- Update stats (years of experience, projects completed)
- Update skills in the skills grid
- Replace email, GitHub, and LinkedIn links

**projects.html:**
- Update project cards with your actual projects
- Add/remove projects as needed
- Update links to your deployed apps
- Replace placeholder images with actual screenshots

### 2. Personalize the Logo

In both HTML files, change the logo from "YN" to your initials:
```html
<a href="index.html" class="logo">YN</a>  <!-- Change this -->
```

### 3. Add Your Projects

For each project:
1. Copy `projects/project-template.html`
2. Rename it (e.g., `streamlit-dashboard.html`)
3. Fill in your project details
4. Update the link in `projects.html`

### 4. Add Project Images

Replace the placeholder divs in `projects.html` with actual images:
```html
<!-- Replace this: -->
<div class="placeholder-image">Project Name</div>

<!-- With this: -->
<img src="images/project-screenshot.png" alt="Project Name">
```

Create an `images/` folder and add your screenshots.

### 5. Customize Colors (Optional)

Edit the CSS variables in `css/style.css`:
```css
:root {
    --color-bg: #0a0a0a;           /* Background color */
    --color-text: #e8e8e8;         /* Text color */
    --color-highlight: #d4af37;    /* Accent color (currently gold) */
    /* ... */
}
```

### 6. Change Fonts (Optional)

The site uses:
- **Display/Headers**: Darker Grotesque
- **Body text**: Crimson Pro

To change fonts, update the Google Fonts link in the HTML files and the CSS variables.

## Deployment to GitHub Pages

### Step 1: Create a GitHub Repository
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### Step 2: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll to "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"

Your site will be live at: `https://yourusername.github.io`

### Step 3: Custom Domain (Optional)
If you have a custom domain:
1. Add a `CNAME` file with your domain name
2. Configure DNS settings with your domain provider
3. Update the custom domain in GitHub Pages settings

## Embedding Your Apps

### For Streamlit Apps:
```html
<iframe src="https://your-app.streamlit.app" 
        width="100%" 
        height="600" 
        frameborder="0">
</iframe>
```

### For Shiny Apps:
```html
<iframe src="https://your-app.shinyapps.io/app-name" 
        width="100%" 
        height="600" 
        frameborder="0">
</iframe>
```

### For Notebooks/HTML Exports:
1. Export your notebook as HTML
2. Place in the `projects/` folder
3. Link to it from `projects.html`

## Tips for Best Results

1. **High-Quality Screenshots**: Use clear, high-resolution images for your projects
2. **Descriptive Text**: Write clear, concise descriptions of what each project does
3. **Keep it Updated**: Regularly add new projects and remove outdated ones
4. **Mobile Testing**: Always check how your site looks on mobile devices
5. **Fast Loading**: Optimize images to keep the site loading quickly
6. **Analytics**: Consider adding Google Analytics to track visitors

## Project Categories

The filtering system supports these categories:
- `apps` - Web applications (Streamlit, Shiny, etc.)
- `analysis` - Data analysis projects
- `viz` - Data visualizations

Update the `data-category` attribute in `projects.html` to match your projects.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

Feel free to use this template for your own portfolio. No attribution required.

## Questions?

If you need help customizing this portfolio, feel free to reach out or open an issue.

---

**Happy building! 🚀**