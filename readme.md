### File Structure
```
strong-humans-foundation/
├── index.html          # Main website file
├── README.md          # This file
├── package.json       # Project metadata
├── CNAME             # Custom domain (optional)
└── images/           # Create this folder for your images
    ├── background.mp4                     # Hero video background
    ├── video-poster.jpg                   # Video poster/fallback image (optional)
    ├── strong-humans-logo.png
    ├── surf-brigade-logo.png
    ├── coast-iii-coast-logo.png
    ├── gallery-1.jpg     # Activity therapy showcase
    ├── gallery-5.jpg     # Diverse therapeutic activities
    ├── army-photo-1.jpg  # Military history photo 1 (horizontal)
    ├── army-photo-2.jpg  # Military history photo 2 (horizontal)
    └── army-photo-3.jpg  # Military history photo 3 (horizontal)
```# Strong Humans Foundation Website

A professional, modern website for the Strong Humans Foundation - a non-profit organization dedicated to empowering veterans, first responders, and their families through wellness initiatives.

![Strong Humans Foundation](https://img.shields.io/badge/version-1.0.0-green.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

## 🌟 Features

- **Single Page Application**: Fast, smooth navigation with no page reloads
- **Full-Screen Video Background**: Immersive hero section with background.mp4
- **Floating Transparent Header**: Modern glassmorphic navigation bar that adapts on scroll
- **Professional Typography**: Montserrat headings, Lato body text, Source Serif Pro accents
- **Vibrant Color Scheme**: Professional design with navy, red, green, and gold accents
- **Partners Section**: Unique coral-colored section with horizontal partner display
- **Multiple Gallery Sections**: Activity therapy and diverse therapeutic activities
- **PayPal Donation Integration**: Direct link to PayPal donation page with email instructions
- **A History of Strength**: Military service photo gallery with 3 horizontal images
- **Responsive Design**: Looks great on all devices (desktop, tablet, mobile)
- **Contact Form**: Ready-to-use contact form with styled info cards
- **Animated Elements**: Subtle animations including floating backgrounds and hover effects
- **Programs Ticker**: Professional scrolling banner with therapy programs
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
2. **Add your images** to this folder (including partner logos)
3. **Replace the placeholder content** with your image tag:

```html
<!-- Before (Header Logo) -->
<div class="logo-circle">
    <div class="logo-placeholder">SH</div>
</div>

<!-- After -->
<div class="logo-circle">
    <img src="images/strong-humans-retreat-logo.png" alt="Strong Humans Retreat">
</div>

<!-- Before (Partner Logo) -->
<div class="partner-logo">
    <div class="partner-placeholder">SB</div>
</div>

<!-- After -->
<div class="partner-logo">
    <img src="images/surf-brigade-logo.png" alt="Surf Brigade">
</div>
```

### Recommended Image Locations:

- **Hero Video**: Add your background.mp4 video file (full-screen background)
- **Logo**: Add your Strong Humans Retreat logo in the header circle (45x45px)
- **Partners Section**: Add partner logos (Surf Brigade, Coast III Coast) - 180x180px recommended
- **Gallery Images**: 
  - gallery-1.jpg - Activity therapy showcase
  - gallery-5.jpg - Diverse therapeutic activities
- **Military History Photos**: Add 3 horizontal army photos for "A History of Strength" section
  - army-photo-1.jpg (16:9 aspect ratio recommended)
  - army-photo-2.jpg (16:9 aspect ratio recommended)
  - army-photo-3.jpg (16:9 aspect ratio recommended)

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
        <a href="#" class="news-link">Read More →</a>
    </div>
</div>
```

### 3. **Adding More Partners**
To add additional partners, copy this template and add it to the partners-grid:
```html
<div class="partner-card">
    <div class="partner-logo">
        <img src="images/new-partner-logo.png" alt="Partner Name">
    </div>
    <p class="partner-name">Partner Name</p>
</div>
```

### 4. **Modifying Colors**
Edit the CSS variables at the top of the file:
```css
:root {
    --primary-navy: #0B1929;      /* Deep navy blue */
    --vibrant-red: #D73528;       /* Strong red accent */
    --forest-green: #2A5F3F;      /* Deep green */
    --warm-gold: #F4A460;         /* Golden highlights */
    --sky-blue: #5B9BD5;          /* Light blue accents */
    --sand: #F5E6D3;              /* Warm sand background */
}
```

### 5. **Adding New Sections**
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
    ├── background.mp4                     # Hero video background
    ├── video-poster.jpg                   # Video poster/fallback image
    ├── strong-humans-retreat-logo.png
    ├── partners/
    │   ├── surf-brigade-logo.png
    │   └── coast-iii-coast-logo.png
    └── gallery/
        ├── gallery-1.jpg
        ├── photo-2.jpg
        ├── photo-3.jpg
        ├── photo-4.jpg
        └── gallery-5.jpg
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
   - Use `.png` for logos with transparency (especially partner logos)
   - Compress images before uploading (use TinyPNG or similar)
   - Keep images under 200KB when possible
   - Partner logos should have transparent backgrounds

2. **Consistent Styling**:
   - The vibrant color scheme uses navy, red, green, and gold
   - Maintain these colors throughout any additions
   - Use the existing CSS classes for consistency
   - Test on mobile devices after changes

3. **Content Guidelines**:
   - Keep text concise and impactful
   - Use active voice
   - Include calls-to-action
   - Update news/events regularly
   - Highlight partner contributions

## 🤝 Need Help?

If you need assistance:
1. Check the comments in the HTML file
2. Refer to the CSS classes for styling options
3. Test locally before pushing to GitHub

## 📄 License

This project is licensed under the MIT License - feel free to customize and use for your organization.

---

Built with ❤️ for the Strong Humans Foundation