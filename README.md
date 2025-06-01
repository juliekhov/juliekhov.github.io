# Nautical Dream Portfolio Website

A modern, responsive portfolio website for nauticaldream.me featuring multiple project pages with a nautical theme.

## 🌊 Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Single Page Application**: Smooth navigation without page reloads
- **Project Showcase**: Dedicated pages for individual projects with detailed information
- **Modern UI**: Clean design with nautical-inspired colors and animations
- **GitHub Pages Ready**: Optimized for deployment on GitHub Pages

## 🚀 Quick Setup for GitHub Pages

### Option 1: Direct Deployment
1. Fork or create a new repository named `username.github.io` (replace `username` with your GitHub username)
2. Copy the `index.html` file to the root of your repository
3. Commit and push the changes
4. Your site will be available at `https://username.github.io`

### Option 2: Custom Domain (nauticaldream.me)
1. Create a repository (can be named anything, e.g., `nautical-dream-website`)
2. Copy the `index.html` file to the root
3. Create a `CNAME` file in the root directory with the content: `nauticaldream.me`
4. In your repository settings:
   - Go to Pages section
   - Set source to "Deploy from a branch"
   - Select "main" branch and "/ (root)" folder
5. Configure your domain's DNS settings to point to GitHub Pages

## 📁 File Structure
```
nauticaldream.me/
├── index.html          # Main website file (single-page application)
├── CNAME              # Domain configuration for GitHub Pages
└── README.md          # This documentation file
```

## 🎨 Customization Guide

### Adding New Projects
To add a new project to the portfolio:

1. **Add to Projects Grid**: Find the `.projects-grid` sections in both the home and projects pages, then add:
```html
<div class="project-card" onclick="showProject('your-project-id')">
    <div class="project-image">🆕</div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <p>Brief description of your project.</p>
        <div class="project-tech">
            <span class="tech-tag">Technology 1</span>
            <span class="tech-tag">Technology 2</span>
        </div>
    </div>
</div>
```

2. **Add Project Detail Page**: Add a new page section:
```html
<div id="your-project-id" class="page project-detail">
    <button class="back-btn" onclick="showPage('projects')">← Back to Projects</button>
    <h2>Your Project Name</h2>
    <div class="meta">
        <div class="meta-item">
            <span class="meta-label">Timeline</span>
            <span class="meta-value">X months</span>
        </div>
        <!-- Add more meta information -->
    </div>
    <p>Detailed project description...</p>
</div>
```

### Changing Colors and Styling
The main color scheme uses CSS custom properties. Key colors to modify:
- **Primary Blue**: `#3498db`
- **Dark Blue**: `#2c3e50`
- **Light Gray**: `#7f8c8d`
- **Background**: `linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%)`

### Updating Content
- **Site Title**: Change "Nautical Dream" in the header
- **About Section**: Update the content in the `#about` page
- **Contact Information**: Modify the contact details in the `#contact` page
- **Hero Section**: Update the welcome message on the home page

## 🔧 Technical Details

### Technologies Used
- **HTML5**: Semantic markup structure
- **CSS3**: Modern styling with Flexbox and Grid
- **Vanilla JavaScript**: Client-side navigation and interactivity
- **Responsive Design**: Mobile-first approach with media queries

### Browser Support
- Chrome/Edge: Full support
- Firefox: Full support  
- Safari: Full support
- Mobile browsers: Optimized for iOS Safari and Chrome Mobile

### Performance Features
- **Lightweight**: Single HTML file under 50KB
- **Fast Loading**: No external dependencies
- **Smooth Animations**: CSS transitions and transforms
- **SEO Friendly**: Semantic HTML structure

## 🌐 Domain Configuration

### DNS Settings for nauticaldream.me
Configure your domain registrar with these DNS records:
```
Type: CNAME
Name: www
Value: username.github.io

Type: A
Name: @
Value: 185.199.108.153
Value: 185.199.109.153
Value: 185.199.110.153
Value: 185.199.111.153
```

### CNAME File
Create a `CNAME` file in your repository root:
```
nauticaldream.me
```

## 📱 Mobile Optimization

The website is fully responsive and includes:
- Flexible navigation that collapses on mobile
- Touch-friendly buttons and links
- Optimized images and text sizing
- Smooth scrolling and transitions

## 🔒 HTTPS Support

GitHub Pages automatically provides HTTPS for both `github.io` and custom domains. Ensure "Enforce HTTPS" is enabled in your repository settings.

## 📈 Analytics Integration

To add Google Analytics, insert this code before the closing `</head>` tag:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🐛 Troubleshooting

### Common Issues

**Site not loading**: 
- Check that `index.html` is in the repository root
- Verify GitHub Pages is enabled in repository settings

**Custom domain not working**:
- Ensure CNAME file contains only the domain name
- Verify DNS records are correctly configured
- Allow up to 24 hours for DNS propagation

**Styling issues on mobile**:
- Clear browser cache
- Test in an incognito/private window

## 🤝 Contributing

To contribute to this project:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly on different devices
5. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Support

For questions or support:
- Email: hello@nauticaldream.me
- Create an issue in this repository
- Check the GitHub Pages documentation

---

**Built with ❤️ for the nautical community**
