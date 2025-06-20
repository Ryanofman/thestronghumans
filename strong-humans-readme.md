# Strong Humans Foundation Website

A professional, modern website for the Strong Humans Foundation - a non-profit organization dedicated to empowering veterans, first responders, and their families through wellness initiatives.

![Strong Humans Foundation](https://img.shields.io/badge/version-1.0.0-green.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

## 🌟 Features

- **Single Page Application**: Fast, smooth navigation with no page reloads
- **Responsive Design**: Looks great on all devices (desktop, tablet, mobile)
- **Easy to Customize**: Well-commented code with clear sections
- **Image Ready**: Marked locations for easy image additions
- **Contact Form**: Ready-to-use contact form (needs backend integration)
- **Smooth Animations**: Professional scroll effects and hover states
- **SEO Friendly**: Semantic HTML structure

## 🚀 Quick Start

### Deploy to GitHub Pages

1. **Fork or Download** this repository
2. **Create a new repository** on GitHub named `your-username.github.io` (if you want it as your main site) or any name for a project site
3. **Upload the files**:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```
4. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Source: Deploy from a branch
   - Branch: main (or master)
   - Folder: / (root)
5. **Visit your site** at `https://your-username.github.io` or `https://your-username.github.io/repository-name`

## 🖼️ Adding Images

The website has clearly marked locations for images. Look for these comments in the HTML:

```html
<!-- Replace with actual image: <img src="path/to/image.jpg" alt="Description"> -->
```

### Steps to Add Images:

1. **Create an `images` folder** in your repository
2. **Add your images** to this folder
3. **Replace the placeholder content** with your image tag:

```html
<!-- Before -->
<div class="testimonial-image">
    <span>ER</span>
</div>

<!-- After -->
<div class="testimonial-image">
    <img src="images/eleanor-ramirez.jpg" alt="Eleanor Ramirez">
</div>
```

### Recommended Image Locations:

- **Testimonials**: Replace initials with profile photos (80x80px recommended)
- **News Cards**: Add featured images for each news story (600x400px recommended)
- **Article Icons**: Replace emoji with custom icons or images
- **Hero Background**: Add a hero image by modifying the `.hero` CSS class

## 📝 Customizing Content

### 1. **Organization Info**
Update contact information in the Contact Section:
```html
<span class="info-label">Phone:</span> YOUR-PHONE-NUMBER
<span class="info-label">Email:</span> your-email@domain.org
<span class="info-label">Address:</span> Your Address Here
```

### 2. **Adding News/Events**
Copy and modify this template:
```html
<div class="news-card">
    <div class="news-image add-image-here">
        <img src="images/your-event.jpg" alt="Event Name">
    </div>
    <div class="news-content">
        <p class="news-date">Month DD, YYYY</p>
        <h3 class="news-title">Your Event Title</h3>
        <p class="news-excerpt">Brief description of the event...</p>
        <a href="#" class="news-link">More →</a>
    </div>
</div>
```

### 3. **Modifying Colors**
Edit the CSS variables at the top of the file:
```css
:root {
    --primary-color: #2c5f2d;      /* Main green - change this */
    --secondary-color: #97bc62;     /* Light green - change this */
    --accent-color: #4a7c59;        /* Dark green - change this */
}
```

### 4. **Adding New Sections**
To add a new section, use this template:
```html
<section class="your-section-name" id="unique-id">
    <div class="section-container">
        <h2 class="section-title">Section Title</h2>
        <!-- Your content here -->
    </div>
</section>
```

## 🔧 Technical Details

### File Structure
```
strong-humans-foundation/
├── index.html          # Main website file
├── README.md          # This file
├── package.json       # Project metadata
├── CNAME             # Custom domain (optional)
└── images/           # Create this folder for your images
    ├── hero.jpg
    ├── testimonials/
    ├── news/
    └── icons/
```

### Form Integration
The contact form requires backend integration. Options:
- **Formspree**: Simple form backend (https://formspree.io)
- **Netlify Forms**: If hosting on Netlify
- **EmailJS**: Client-side email sending
- **Custom Backend**: Your own server solution

Example with Formspree:
```html
<form action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
```

## 🎨 Design Tips

1. **Image Optimization**:
   - Use `.jpg` for photos
   - Use `.png` for logos/icons with transparency
   - Compress images before uploading (use TinyPNG or similar)
   - Keep images under 200KB when possible

2. **Consistent Styling**:
   - Maintain the color scheme throughout
   - Use the existing CSS classes for consistency
   - Test on mobile devices after changes

3. **Content Guidelines**:
   - Keep text concise and impactful
   - Use active voice
   - Include calls-to-action
   - Update news/events regularly

## 🤝 Need Help?

If you need assistance:
1. Check the comments in the HTML file
2. Refer to the CSS classes for styling options
3. Test locally before pushing to GitHub

## 📄 License

This project is licensed under the MIT License - feel free to customize and use for your organization.

---

Built with ❤️ for the Strong Humans Foundation