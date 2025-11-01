# Portfolio Website

A modern, responsive portfolio website built with HTML, CSS, and JavaScript.

## Features

- ✨ Modern and clean design
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎨 Smooth animations and transitions
- 🚀 Fast and optimized
- ♿ Accessible
- 📧 Contact form ready for integration

## Sections

1. **Hero Section** - Eye-catching introduction with your name and title
2. **About** - Personal introduction and statistics
3. **Skills** - Technical skills organized by category
4. **Experience** - Work experience timeline
5. **Education** - Educational background
6. **Projects** - Portfolio of your work
7. **Contact** - Contact information and form

## Customization Guide

### 1. Update Personal Information

**In `index.html`:**

- **Hero Section**: Update name, title, and description
  ```html
  <span class="name">Your Name</span>
  <span class="title">Your Title</span>
  ```

- **About Section**: Replace placeholder text with your bio
- **Contact Section**: Update email, phone, and location
- **Social Links**: Add your social media profiles

### 2. Update Skills

Replace the skill items in the Skills section:

```html
<span class="skill-item">Your Skill</span>
```

### 3. Add Your Experience

Update the timeline items in the Experience section:

```html
<div class="timeline-item">
    <div class="timeline-date">2023 - Present</div>
    <h3 class="timeline-title">Your Position</h3>
    <h4 class="timeline-company">Company Name</h4>
    <!-- Add your responsibilities -->
</div>
```

### 4. Add Your Projects

Update project cards with your actual projects:

```html
<div class="project-card">
    <div class="project-content">
        <h3 class="project-title">Your Project</h3>
        <p class="project-description">Project description</p>
        <!-- Add project links and tags -->
    </div>
</div>
```

### 5. Add Your Photo

Replace the placeholder in the About section:

```html
<div class="about-image">
    <img src="path/to/your/photo.jpg" alt="Your Name">
</div>
```

Update CSS:

```css
.about-image img {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    object-fit: cover;
}
```

### 6. Customize Colors

In `styles.css`, update the CSS variables:

```css
:root {
    --primary-color: #6366f1;    /* Your primary color */
    --secondary-color: #ec4899;  /* Your secondary color */
    /* ... other variables */
}
```

### 7. Add Project Images

Replace placeholders with actual project images:

```html
<div class="project-image">
    <img src="path/to/project-image.jpg" alt="Project Name">
    <div class="project-overlay">...</div>
</div>
```

### 8. Connect Contact Form

The form is ready but needs backend integration. Options:

- **EmailJS**: Easy email service integration
- **Formspree**: Simple form backend
- **Netlify Forms**: If hosting on Netlify
- **Custom Backend**: Your own server endpoint

Example with EmailJS:

```javascript
// Install EmailJS first: npm install @emailjs/browser

import emailjs from '@emailjs/browser';

contactForm.addEventListener('submit', async (e) => {
    e.preventDefault();
    
    emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', contactForm, 'YOUR_PUBLIC_KEY')
        .then(() => {
            alert('Message sent successfully!');
            contactForm.reset();
        });
});
```

## File Structure

```
portfolio/
├── index.html      # Main HTML file
├── styles.css      # All styles
├── script.js       # JavaScript functionality
└── README.md       # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance Tips

1. Optimize images before adding them
2. Use WebP format for better compression
3. Minimize custom fonts if used
4. Consider lazy loading for images

## Deployment

### Netlify (Recommended)

1. Create a Netlify account
2. Connect your repository or drag & drop the folder
3. Your site will be live!

### GitHub Pages

1. Push your code to a GitHub repository
2. Go to Settings > Pages
3. Select your branch and folder
4. Your site will be available at `username.github.io/repository-name`

### Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts

## Credits

- Font Awesome Icons
- Modern CSS techniques
- Vanilla JavaScript

## License

Feel free to use this template for your personal portfolio!

---

**Need help?** Feel free to reach out or open an issue!

