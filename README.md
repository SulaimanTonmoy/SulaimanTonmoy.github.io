# Engineering Portfolio - GitHub.io

A modern, interactive portfolio website designed for engineers and recruiting professionals. Built with cutting-edge web technologies and featuring smooth animations, responsive design, and professional aesthetics.

## 🚀 Features

- **Modern UI/UX Design**: Clean, professional interface with gradient accents and smooth animations
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Interactive Animations**: 
  - Typing animation for role titles
  - Floating particle effects
  - Scroll-triggered animations using AOS
  - Parallax scrolling effects
  - Hover animations and micro-interactions
- **Professional Sections**:
  - Hero section with animated introduction
  - About section with personal information
  - Skills showcase with animated progress bars
  - Projects gallery with interactive cards
  - Experience timeline
  - Contact form with validation
- **Performance Optimized**: Lazy loading, debounced events, and efficient animations
- **SEO Friendly**: Semantic HTML5 structure and meta tags
- **Easy Customization**: Well-organized code for easy editing

## 🛠️ Technologies Used

- **HTML5**: Semantic markup and modern structure
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Vanilla JavaScript**: Interactive features and animations
- **AOS (Animate On Scroll)**: Scroll animation library
- **Font Awesome**: Professional icons
- **Google Fonts**: Typography (if needed)

## 📁 Project Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # Custom CSS and animations
├── script.js           # JavaScript functionality
├── README.md           # This file
└── assets/             # Images and other assets (if needed)
```

## 🚀 Quick Start

### Local Development

1. **Clone or download the repository**
   ```bash
   git clone <repository-url>
   cd portfolio
   ```

2. **Open in browser**
   Simply open `index.html` in your web browser, or use a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (if you have http-server installed)
   npx http-server
   
   # Using VS Code Live Server extension
   Right-click index.html → Open with Live Server
   ```

3. **Visit the site**
   Navigate to `http://localhost:8000` (or your chosen port)

## 🌐 Custom Domain Setup

### For sulaimanhossain.online

1. **Create CNAME file** (already included):
   ```
   sulaimanhossain.online
   ```

2. **DNS Configuration**:
   - Go to your domain registrar (where you bought sulaimanhossain.online)
   - Add a CNAME record pointing to: `username.github.io` (replace with your GitHub username)
   - Or add an A record pointing to GitHub Pages IP addresses:
     - `185.199.108.153`
     - `185.199.109.153` 
     - `185.199.110.153`
     - `185.199.111.153`

3. **GitHub Pages Settings**:
   - Go to repository Settings → Pages
   - Under "Custom domain", enter: `sulaimanhossain.online`
   - Check "Enforce HTTPS"
   - Save

4. **Wait for DNS Propagation**:
   - DNS changes may take 24-48 hours to propagate
   - GitHub will automatically verify your domain

### GitHub Pages Deployment

### Method 1: Direct Repository Upload

1. **Create a new repository** on GitHub named `username.github.io` (replace `username` with your GitHub username)

2. **Upload files** to the repository:
   - Drag and drop all files to the repository
   - Or clone the repository and push the files

3. **Visit your site** at `https://username.github.io`

### Method 2: Using GitHub Pages from Any Repository

1. **Push your code** to any GitHub repository

2. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: main (or master) → / (root)
   - Click Save

3. **Visit your site** at the URL shown in the Pages settings

## ✏️ Customization Guide

### Personal Information

Edit `index.html` and update the following:

1. **Personal Details** (lines 25-35):
   ```html
   <h1>John Doe</h1>
   <p>john.doe@example.com</p>
   <!-- Update social media links -->
   ```

2. **About Section** (lines 80-120):
   ```html
   <p>Your personal description...</p>
   <!-- Update education, experience, location, interests -->
   ```

3. **Skills** (lines 140-200):
   ```html
   <!-- Update skill names and percentages -->
   <div class="skill-item">
       <span>Your Skill</span>
       <div style="width: 90%"></div>
   </div>
   ```

4. **Projects** (lines 220-320):
   ```html
   <!-- Update project information, links, and technologies -->
   <div class="project-card">
       <h3>Your Project Name</h3>
       <p>Project description...</p>
   </div>
   ```

5. **Experience** (lines 340-450):
   ```html
   <!-- Update work experience timeline -->
   <div class="timeline-item">
       <h3>Your Job Title</h3>
       <h4>Company Name</h4>
       <p>Job description...</p>
   </div>
   ```

6. **Contact Information** (lines 470-520):
   ```html
   <!-- Update email, phone, and social links -->
   <span>your.email@example.com</span>
   ```

### Styling Customization

Edit `styles.css` to modify:

- **Colors**: Update gradient colors and theme colors
- **Animations**: Adjust timing, easing, and effects
- **Typography**: Change fonts and text styles
- **Layout**: Modify spacing and responsive breakpoints

### JavaScript Features

Edit `script.js` to:

- **Typing Animation**: Update role titles in the `roles` array
- **Particle Effects**: Adjust particle count and behavior
- **Form Handling**: Replace with your actual form submission logic
- **Analytics**: Add your analytics tracking code

## 🎨 Design System

### Color Palette
- **Primary Blue**: `#3b82f6`
- **Primary Purple**: `#8b5cf6`
- **Dark Background**: `#0f172a`
- **Card Background**: `#1f2937`
- **Text Primary**: `#ffffff`
- **Text Secondary**: `#9ca3af`

### Typography
- **Headings**: Bold, gradient text effects
- **Body**: Clean, readable sans-serif
- **Code**: Monospace for technical content

### Animations
- **Duration**: 0.3s - 2s depending on complexity
- **Easing**: Primarily `ease` and `ease-out`
- **Performance**: GPU-accelerated transforms

## 📱 Responsive Breakpoints

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## 🚀 Performance Tips

1. **Optimize Images**: Compress images before uploading
2. **Minimize Assets**: Consider minifying CSS/JS for production
3. **Enable Caching**: Configure proper cache headers
4. **Use CDN**: Host assets on CDN for faster loading

## 🔧 Advanced Customizations

### Adding New Sections

1. **HTML Structure**:
   ```html
   <section id="new-section" class="py-20">
       <div class="container mx-auto px-6">
           <!-- Your content -->
       </div>
   </section>
   ```

2. **Navigation Update**:
   ```html
   <a href="#new-section" class="nav-link">New Section</a>
   ```

### Custom Animations

Add new animations to `styles.css`:
```css
@keyframes yourAnimation {
    0% { /* Start state */ }
    100% { /* End state */ }
}

.your-element {
    animation: yourAnimation 2s ease infinite;
}
```

## 🐛 Troubleshooting

### Common Issues

1. **Animations not working**: Check browser console for JavaScript errors
2. **Mobile menu not opening**: Verify JavaScript is loaded and no conflicts
3. **Form not submitting**: Check form validation and network requests
4. **Styling issues**: Clear browser cache and check CSS specificity

### Browser Compatibility

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📞 Support

If you need help with customization or deployment:
1. Check this README thoroughly
2. Search existing GitHub issues
3. Create a new issue with detailed information

---

**Built with ❤️ for engineers and recruiters**
