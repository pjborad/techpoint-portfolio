# Pritesh Borad - Portfolio Website

A modern, responsive personal portfolio website showcasing data science expertise, projects, skills, and professional experience.

[![Live Demo](https://img.shields.io/badge/demo-live-green.svg)](https://your-portfolio-url.com)
[![GitHub](https://img.shields.io/badge/GitHub-pjborad-blue.svg)](https://github.com/pjborad)

## 🎯 Overview

This is a single-page portfolio website built with vanilla HTML, CSS, and JavaScript. It features a clean, modern design with smooth scrolling navigation, responsive layouts, and custom animations.

## ✨ Features

- **Responsive Design**: Fully responsive across all devices (desktop, tablet, mobile)
- **Single Page Application**: Smooth scrolling navigation between sections
- **Custom Fonts**: Three custom font families (General Sans, Okine Sans, Satoshi)
- **Interactive Elements**: Hamburger menu for mobile navigation
- **Progress Bars**: Animated skill level indicators
- **Social Media Integration**: Links to GitHub, LinkedIn, and email
- **SEO Optimized**: Meta tags for social media sharing and search engines

## 📋 Sections

1. **Hero/Landing**: Introduction with call-to-action buttons
2. **About**: Personal introduction and professional summary
3. **Services**: Services offered (section placeholder)
4. **Projects**: Featured and notable projects with descriptions
5. **Skills**: Technical skills with visual progress indicators
6. **Contact**: Contact information and social media links

## 🚀 Getting Started

### Prerequisites

No installation required! This is a static website that runs directly in any modern web browser.

### Installation & Running

1. **Clone the repository**
   ```bash
   git clone https://github.com/pjborad/techpoint-portfolio.git
   cd techpoint-portfolio
   ```

2. **Open the website**
   
   **Option 1: Double-click** `index.html` to open in your default browser
   
   **Option 2: Use a local server** (recommended for development)
   
   Using Python:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   ```
   
   Using Node.js (http-server):
   ```bash
   npx http-server -p 8000
   ```
   
   Using VS Code Live Server:
   - Install the "Live Server" extension
   - Right-click `index.html` → "Open with Live Server"

3. **View the website**
   - Direct open: File will open in browser
   - Local server: Navigate to `http://localhost:8000`

## 📁 Project Structure

```
techpoint-portfolio/
│
├── index.html              # Main HTML file
├── README.md              # This file
├── LICENSE                # License file
├── CNAME                  # Custom domain configuration
│
├── css/                   # Stylesheets
│   ├── style.css         # Main stylesheet
│   ├── normalize.css     # CSS normalization
│   ├── reset.css         # CSS reset
│   └── font-root-styles/ # Font definitions
│       ├── general-sans.css
│       ├── okinesans.css
│       └── satoshi.css
│
├── js/                    # JavaScript files
│   └── main.js           # Main JavaScript (mobile menu)
│
├── fonts/                 # Custom font files
│   ├── general-sans/
│   ├── okine/
│   └── satoshi/
│
└── img/                   # Images and icons
    ├── profile.jpg        # Profile picture
    ├── github.svg         # GitHub icon
    ├── link.svg          # External link icon
    ├── og-img.png        # Open Graph image
    └── favicon/          # Favicon files
        ├── about.txt
        └── site.webmanifest
```

## 🎨 Customization Guide

### 1. Personal Information

**File**: `index.html`

**Update the following sections:**

- **Meta Tags** (Lines 7-60):
  ```html
  <title>Your Name</title>
  <meta name="description" content="Your description">
  <meta property="og:title" content="Your Name">
  ```

- **Navigation Logo** (Line 101):
  ```html
  <span class="logo">YOUR NAME</span>
  ```

- **Hero Section** (Lines 294-295):
  ```html
  <h1>I am <span class="name-highlight">Your Name</span>.</h1>
  ```

- **About Section** (Lines 476-490): Update your bio and expertise
- **Footer** (Line 1023): Update copyright name

### 2. Social Media Links

**Update in three locations:**
- Navigation menu (Lines 135-285)
- Main social links (Lines 318-468)
- Contact section (Lines 852-1014)

**Replace URLs:**
```html
<!-- GitHub -->
<a href="https://github.com/YOUR-USERNAME" target="_blank">

<!-- LinkedIn -->
<a href="https://www.linkedin.com/in/YOUR-PROFILE/" target="_blank">

<!-- Email -->
<a href="mailto:your-email@example.com">
```

### 3. Projects

**File**: `index.html` (Lines 502-765)

**Update project details:**
```html
<div class="project project1">
  <span>Project #1</span>
  <h3>Your Project Name</h3>
  <p>Your project description</p>
  
  <!-- Update links -->
  <a href="https://github.com/YOUR-USERNAME/YOUR-REPO" target="_blank">
  
  <!-- Update image -->
  <img src="img/your-project-image.png" alt="Project Preview">
  
  <!-- Update technologies -->
  <p>Your, Tech, Stack</p>
</div>
```

### 4. Skills

**File**: `index.html` (Lines 800-851)

**Update skill levels:**
```html
<div class="skill">
  <span>Your Skill</span>
  <div class="progress">
    <div class="progress-bar" style="width: 85%;"></div> <!-- Change percentage -->
    <div class="progress-bar-inactive"></div>
  </div>
</div>
```

### 5. Colors & Styling

**File**: `css/style.css`

**Primary color (Orange highlight)**: Search for `#ffa500` and replace with your color
**Background colors**: Update dark theme colors in the CSS file
**Fonts**: Modify font families in `css/font-root-styles/` directory

### 6. Images

**Add your images to `img/` folder:**
- `profile.jpg` - Your profile picture (About section)
- Project screenshots for each project
- Update all image references in `index.html`

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: 
  - Custom properties (CSS variables)
  - Flexbox layouts
  - CSS animations
  - Media queries for responsiveness
- **JavaScript (ES6)**: Mobile menu toggle functionality
- **Custom Fonts**: General Sans, Okine Sans, Satoshi

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 Key Files to Edit

### Must Edit:
1. `index.html` - All content, personal info, projects, skills
2. `img/profile.jpg` - Your profile picture
3. `CNAME` - Your custom domain (if deploying to GitHub Pages)

### Optional Edit:
1. `css/style.css` - Colors, spacing, custom styles
2. `js/main.js` - Add custom JavaScript functionality
3. `img/` - All project images and icons

## 🚀 Deployment

### GitHub Pages

1. Go to repository Settings → Pages
2. Select branch: `main`
3. Select folder: `/ (root)`
4. Click Save
5. Your site will be live at `https://YOUR-USERNAME.github.io/techpoint-portfolio/`

### Custom Domain

1. Add your domain to `CNAME` file
2. Configure DNS settings with your domain provider
3. Point to GitHub Pages IP addresses

### Netlify/Vercel

1. Connect your GitHub repository
2. Set build command: (none - static site)
3. Set publish directory: `/`
4. Deploy!

## 📧 Contact

- **Email**: priteshborad1998@gmail.com
- **LinkedIn**: [Pritesh Borad](https://www.linkedin.com/in/priteshborad/)
- **GitHub**: [@pjborad](https://github.com/pjborad)

## 📄 License

This project is open source and available under the [LICENSE](LICENSE) file.

## 🙏 Acknowledgments

- Font families: General Sans, Okine Sans, Satoshi
- Icons: Custom SVG icons
- Design inspiration: Modern portfolio trends

---

**Made with ❤️ by Pritesh Borad**

## If you like this project, please give it a 🌟
## Thank you 😊
