# 🚀 How to Recreate My Personal Portfolio Website

## Overview
This guide shows you how to recreate a modern, professional portfolio website similar to [aymanaboghonim.github.io](https://aymanaboghonim.github.io) using Vite, Bootstrap, and GitHub Pages.

## 🎯 What You'll Build
- **Modern Portfolio**: Clean, responsive design with smooth animations
- **Professional Sections**: Hero, About, Experience, Projects, Blog, Contact
- **GitHub Pages Deployment**: Free hosting with custom domain support
- **Fast Loading**: Vite build system for optimized performance
- **Mobile-First**: Responsive design that works on all devices

## 🛠️ Tech Stack
- **Build Tool**: Vite (fast development and build)
- **CSS Framework**: Bootstrap 5 (responsive grid and components)
- **Animations**: AOS (Animate On Scroll)
- **Icons**: Bootstrap Icons
- **Fonts**: Google Fonts (Inter + Fira Code)
- **Deployment**: GitHub Pages

## 📋 Prerequisites
- Node.js (v16 or higher)
- Git and GitHub account
- Basic knowledge of HTML, CSS, and JavaScript

## 🚀 Step-by-Step Recreation

### 1. Project Setup
```bash
# Create new repository on GitHub: yourusername.github.io
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io

# Initialize Vite project
npm init -y
npm install vite sass bootstrap aos
npm install -D gh-pages
```

### 2. Project Structure
```
your-portfolio/
├── src/
│   ├── index.html          # Main HTML file
│   ├── styles/
│   │   └── main.scss      # Custom styles
│   ├── js/
│   │   └── main.js        # JavaScript functionality
│   └── assets/
│       └── img/
│           └── profile.jpg # Your profile image
├── package.json
├── vite.config.js
└── .nojekyll              # Prevents Jekyll processing
```

### 3. Vite Configuration
Create `vite.config.js`:
```javascript
import { defineConfig } from 'vite'

export default defineConfig({
  root: 'src',
  build: {
    outDir: '../dist',
    emptyOutDir: true
  }
})
```

### 4. Package.json Scripts
```json
{
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview",
    "deploy": "npm run build && gh-pages -d dist"
  }
}
```

### 5. HTML Structure Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name - AI/ML Engineer</title>
    <!-- Meta tags for SEO -->
    <!-- Bootstrap Icons -->
    <!-- Google Fonts -->
    <!-- AOS CSS -->
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-light fixed-top bg-white shadow-sm">
        <!-- Navigation content -->
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section d-flex align-items-center min-vh-100">
        <!-- Hero content with profile image and intro -->
    </section>

    <!-- About Section -->
    <section id="about" class="py-5 bg-light">
        <!-- About content -->
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-5">
        <!-- Timeline of experience -->
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-5 bg-light">
        <!-- Project cards -->
    </section>

    <!-- Blog Section -->
    <section id="blog" class="py-5">
        <!-- Blog post cards -->
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-5 bg-light">
        <!-- Contact information and social links -->
    </section>

    <!-- Scripts -->
    <script type="module" src="/js/main.js"></script>
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
</body>
</html>
```

### 6. Key Features to Implement

#### Responsive Navigation
```html
<nav class="navbar navbar-expand-lg navbar-light fixed-top bg-white shadow-sm">
    <div class="container">
        <a class="navbar-brand fw-bold text-primary" href="#home">
            <span class="me-2">🤖</span>Your Name
        </a>
        <!-- Mobile toggle and navigation items -->
    </div>
</nav>
```

#### Hero Section with Profile
```html
<section id="home" class="hero-section d-flex align-items-center min-vh-100">
    <div class="container">
        <div class="row align-items-center">
            <div class="col-lg-6" data-aos="fade-right">
                <h1 class="display-4 fw-bold mb-4">
                    Hi, I'm <span class="text-primary">Your Name</span>
                </h1>
                <!-- Introduction and social links -->
            </div>
            <div class="col-lg-6 text-center" data-aos="fade-left">
                <!-- Profile image -->
            </div>
        </div>
    </div>
</section>
```

#### Project Cards
```html
<div class="card h-100 border-0 shadow project-card">
    <div class="card-body p-4">
        <div class="d-flex justify-content-between align-items-start mb-3">
            <h5 class="card-title">Project Name</h5>
            <i class="bi bi-robot text-primary fs-4"></i>
        </div>
        <p class="card-text text-muted">Project description...</p>
        <div class="mt-auto">
            <div class="d-flex justify-content-between align-items-center">
                <div class="btn-group" role="group">
                    <a href="#" class="btn btn-outline-primary btn-sm">
                        <i class="bi bi-github"></i> Code
                    </a>
                    <a href="#" class="btn btn-outline-primary btn-sm">
                        <i class="bi bi-eye"></i> Demo
                    </a>
                </div>
                <small class="text-muted">Tech Stack</small>
            </div>
        </div>
    </div>
</div>
```

### 7. Custom SCSS Styling
```scss
// main.scss
@import 'bootstrap/scss/bootstrap';

:root {
    --primary-color: #6366f1;
    --secondary-color: #8b5cf6;
}

.hero-section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
}

.project-card {
    transition: transform 0.3s ease;
    
    &:hover {
        transform: translateY(-5px);
    }
}

// Smooth scrolling
html {
    scroll-behavior: smooth;
}

// Custom animations
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
```

### 8. JavaScript Functionality
```javascript
// main.js
import 'bootstrap/dist/js/bootstrap.bundle.min.js';
import '../styles/main.scss';

// Initialize AOS
document.addEventListener('DOMContentLoaded', function() {
    AOS.init({
        duration: 1000,
        once: true
    });
});

// Smooth scrolling for navigation links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});

// Navbar background on scroll
window.addEventListener('scroll', function() {
    const navbar = document.querySelector('.navbar');
    if (window.scrollY > 50) {
        navbar.classList.add('navbar-scrolled');
    } else {
        navbar.classList.remove('navbar-scrolled');
    }
});
```

### 9. Deployment Steps
```bash
# Build and deploy
npm run build

# Copy files to root for GitHub Pages
cp dist/index.html .
cp -r dist/assets .

# Create .nojekyll file
echo "" > .nojekyll

# Commit and push
git add .
git commit -m "Deploy portfolio website"
git push origin master
```

### 10. Customization Tips

#### Personal Branding
- Replace colors in CSS variables
- Update fonts in HTML head
- Add your own emoji/icon in navbar
- Customize animations and transitions

#### Content Sections
- **Experience**: Add your professional timeline
- **Projects**: Showcase your best work with links
- **Skills**: Highlight your technical expertise
- **Blog**: Link to your articles or create a blog section

#### Performance Optimization
- Optimize images (use WebP format)
- Minify CSS and JS in production
- Use CDN for external libraries
- Enable gzip compression

## 🎨 Design Inspiration
- **Color Schemes**: Use tools like Coolors.co
- **Typography**: Google Fonts combinations
- **Animations**: Subtle hover effects and scroll animations
- **Layout**: Mobile-first responsive design

## 📱 Testing Checklist
- [ ] Mobile responsiveness
- [ ] Cross-browser compatibility
- [ ] Loading performance
- [ ] Social media links work
- [ ] Contact form functionality
- [ ] SEO meta tags
- [ ] Accessibility compliance

## 🚀 Enhancement Ideas
- Add dark/light theme toggle
- Implement contact form with Netlify/Formspree
- Add blog with markdown support
- Integrate with CMS (Contentful/Strapi)
- Add analytics (Google Analytics)
- Implement PWA features

## 📚 Resources
- [Vite Documentation](https://vitejs.dev/)
- [Bootstrap 5 Docs](https://getbootstrap.com/docs/5.0/)
- [AOS Animation Library](https://michalsnik.github.io/aos/)
- [GitHub Pages Guide](https://pages.github.com/)

## 🤝 Contributing
Feel free to suggest improvements or share your own portfolio variations!

---

**Pro Tip**: Start with the basic structure and gradually add features. Focus on content first, then enhance with animations and advanced styling.

*Built with ❤️ by [Ayman Aboghonim](https://aymanaboghonim.github.io)*
