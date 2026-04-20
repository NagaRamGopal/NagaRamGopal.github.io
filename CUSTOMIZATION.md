# Portfolio Customization Guide

## Quick Start Checklist

- [ ] Update your name in the hero section
- [ ] Add your professional photo (optional)
- [ ] Update contact information (email, phone, location)
- [ ] Add your actual projects with descriptions
- [ ] Update skills and expertise
- [ ] Add your work experience
- [ ] Add social media links
- [ ] Update color theme if desired
- [ ] Test on mobile devices
- [ ] Deploy to web hosting

---

## Step-by-Step Customization

### 1. Update Hero Section

**File**: `index.html` (Lines 32-47)

Change:
```html
<h1 class="hero-title">
    <span class="gradient-text">Crafting Digital Excellence</span>
</h1>
<p class="hero-subtitle">Full Stack Developer | UI/UX Enthusiast | Problem Solver</p>
<p class="hero-description">
    Transforming ideas into elegant, scalable solutions with cutting-edge technology and design thinking.
</p>
```

To your own headline, subtitle, and description.

### 2. Update About Section

**File**: `index.html` (Lines 82-105)

Replace the placeholder text with your real background, skills, and personality.

### 3. Update Professional Stats

**File**: `index.html` (Lines 115-127)

Update the numbers and labels:
```html
<div class="stat">
    <h3>50+</h3>  <!-- Change this number -->
    <p>Projects Completed</p>  <!-- Change this text -->
</div>
```

### 4. Update Code Block

**File**: `index.html` (Lines 128-139)

Customize the code snippet to match your style:
```html
<p>{ <span class="highlight">name</span>: <span class="string">"Your Name"</span>,</p>
<p style="margin-left: 20px;"><span class="highlight">skills</span>: [<span class="string">"Skill1"</span>, <span class="string">"Skill2"</span>],</p>
```

### 5. Update Skills

**File**: `index.html` (Lines 152-189)

Add your actual skills:
```html
<div class="skill-category">
    <h3><i class="fas fa-code"></i> Your Category</h3>
    <div class="skill-tags">
        <span class="skill-tag">Your Skill 1</span>
        <span class="skill-tag">Your Skill 2</span>
        <span class="skill-tag">Your Skill 3</span>
    </div>
</div>
```

### 6. Update Projects

**File**: `index.html` (Lines 192-287)

For each project, update:
```html
<div class="project-card">
    <div class="project-image">
        <div class="project-placeholder">
            <i class="fas fa-ICON"></i>  <!-- Change icon -->
        </div>
        <div class="project-overlay">
            <a href="YOUR_LIVE_LINK" class="project-btn" title="Live Demo">
                <i class="fas fa-external-link-alt"></i>
            </a>
            <a href="YOUR_GITHUB_LINK" class="project-btn" title="Source Code">
                <i class="fas fa-github"></i>
            </a>
        </div>
    </div>
    <div class="project-info">
        <h3>Your Project Title</h3>
        <p>Your project description</p>
        <div class="project-tags">
            <span>Technology 1</span>
            <span>Technology 2</span>
        </div>
    </div>
</div>
```

**Icon Options**:
- Shopping: `fa-shopping-cart`
- Tasks: `fa-tasks`
- Analytics: `fa-chart-line`
- Learning: `fa-book`
- Map: `fa-map`
- Chat: `fa-comments`
- Camera: `fa-camera`
- Rocket: `fa-rocket`

See full list: https://fontawesome.com/search

### 7. Update Experience

**File**: `index.html` (Lines 310-369)

Update for each job:
```html
<div class="timeline-item">
    <div class="timeline-dot"></div>
    <div class="timeline-content">
        <h3>Your Job Title</h3>
        <p class="timeline-company">Company Name | 2024 - Present</p>
        <p>Your job description</p>
        <ul class="achievements">
            <li>Achievement 1</li>
            <li>Achievement 2</li>
            <li>Achievement 3</li>
        </ul>
    </div>
</div>
```

### 8. Update Contact Information

**File**: `index.html` (Lines 383-406)

Update your email, phone, and location:
```html
<p><a href="mailto:YOUR_EMAIL@gmail.com">YOUR_EMAIL@gmail.com</a></p>
<p><a href="tel:+1XXXXXXXXXX">+1 (XXX) XXX-XXXX</a></p>
<p>Your City, State</p>
```

### 9. Update Contact Form

**File**: `index.html` (Lines 408-417)

Currently, the form shows a success message. To enable email functionality, integrate with:
- **Formspree** (easiest)
- **EmailJS**
- **Backend API**

For Formspree:
```html
<form class="contact-form" method="POST" action="https://formspree.io/f/YOUR_FORM_ID">
    <div class="form-group">
        <input type="text" name="name" placeholder="Your Name" required>
    </div>
    <div class="form-group">
        <input type="email" name="email" placeholder="Your Email" required>
    </div>
    <div class="form-group">
        <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
    </div>
    <button type="submit" class="btn btn-primary">Send Message</button>
</form>
```

### 10. Update Social Links

**File**: `index.html` (Lines 420-439)

Update with your profile links:
```html
<div class="social-links">
    <a href="https://github.com/YOUR_USERNAME" class="social-link" title="GitHub">
        <i class="fab fa-github"></i>
    </a>
    <a href="https://linkedin.com/in/YOUR_PROFILE" class="social-link" title="LinkedIn">
        <i class="fab fa-linkedin"></i>
    </a>
    <!-- Add more social links as needed -->
</div>
```

---

## Color Customization

To change the color scheme, edit `styles.css` (Lines 8-21):

```css
:root {
    --primary-color: #00d4ff;      /* Cyan - Change this */
    --primary-dark: #0099cc;
    --secondary-color: #ff006e;    /* Pink - Change this */
    --bg-dark: #0a0e27;            /* Dark BG - Change this */
    --bg-darker: #050812;          /* Darker BG */
    --text-primary: #e8eef5;       /* Light text */
    --text-secondary: #a8aec8;     /* Gray text */
}
```

**Color Palette Ideas**:
- Professional: Blue (#3b82f6) + Orange (#f59e0b)
- Modern: Purple (#8b5cf6) + Pink (#ec4899)
- Tech: Green (#10b981) + Blue (#0ea5e9)
- Corporate: Navy (#1e3a8a) + Gold (#f59e0b)

---

## Font Customization

To change fonts, edit `styles.css` (Line 47):

```css
body {
    font-family: 'Your Font Name', sans-serif;
}
```

**Google Fonts Recommendations**:
```html
<!-- Add to <head> section in index.html -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
```

Then update CSS:
```css
body {
    font-family: 'Poppins', sans-serif;
}
```

---

## Advanced Customizations

### Add Background Images

In `styles.css`, update hero section:
```css
.hero {
    background: 
        linear-gradient(135deg, var(--bg-darker) 0%, #1a0033 100%),
        url('path-to-your-image.jpg');
    background-size: cover;
    background-position: center;
}
```

### Add Portfolio Images

Replace project placeholder icons with actual images:
```html
<div class="project-image">
    <img src="path-to-your-image.png" alt="Project Name">
</div>
```

### Add Profile Photo

Add to about section:
```html
<div class="hero-visual">
    <img src="path-to-your-photo.jpg" alt="Profile" style="border-radius: 15px; max-width: 100%; box-shadow: var(--shadow-glow);">
</div>
```

---

## Performance Tips

1. **Compress Images**: Use tools like TinyPNG before adding images
2. **Minimize CSS/JS**: Remove unused code
3. **Lazy Loading**: Add `loading="lazy"` to images
4. **Cache Busting**: Add version number to stylesheets

---

## Testing Checklist

- [ ] Mobile responsiveness (test on real devices)
- [ ] Cross-browser compatibility (Chrome, Firefox, Safari, Edge)
- [ ] Contact form functionality
- [ ] Social links work correctly
- [ ] All images load properly
- [ ] Animations are smooth
- [ ] Links point to correct pages
- [ ] No console errors
- [ ] Page loads quickly
- [ ] Accessibility (keyboard navigation, contrast)

---

## Deployment

### GitHub Pages
1. Create repo named `username.github.io`
2. Push portfolio files
3. Enable Pages in settings
4. Live at `https://username.github.io`

### Netlify
1. Connect GitHub repository
2. Set build command to empty (static site)
3. Automatic deployment on push

### Custom Domain
Purchase domain and point DNS to your hosting provider.

---

## Need Help?

- **Font Awesome Icons**: https://fontawesome.com
- **CSS Gradients**: https://cssgradient.io
- **Color Picker**: https://coolors.co
- **Font Selection**: https://fonts.google.com

---

Happy customizing! 🎉
