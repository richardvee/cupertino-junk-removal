# Cupertino Junk Removal Landing Page - Maintenance Guide

This guide will help you maintain and customize the Cupertino Junk Removal landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To modify:

1. **Company Name:**
```html
<a href="/" class="text-2xl font-bold text-emerald-600">
    Cupertino Junk <!-- Change this text -->
</a>
```

2. **Navigation Menu Items:**
```html
<div class="hidden md:flex space-x-8">
    <a href="#services">Services</a> <!-- Change menu item text here -->
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-6">
    Cupertino Junk Removal - Fast, Reliable Waste Hauling Services
    <!-- Edit this headline -->
</h1>
```

#### Tailwind CSS Class Guide
- Text sizes: `text-4xl` (large), `text-2xl` (medium), `text-lg` (regular)
- Colors: `text-emerald-600` (green), `text-gray-900` (dark gray)
- Spacing: `mb-6` (margin bottom), `py-4` (padding top/bottom)
- Responsive design: `md:text-5xl` (applies at medium screens)

### Features Section
Each feature card follows this structure:
```html
<div class="bg-white rounded-xl shadow-lg p-8">
    <div class="w-16 h-16 bg-emerald-100 rounded-full">
        <i class="fas fa-clock"></i> <!-- Change icon here -->
    </div>
    <h3>Same-Day Service</h3> <!-- Change feature title -->
    <p>Quick response times...</p> <!-- Change description -->
</div>
```

## Managing Links

### Navigation Menu Links
Current links in the navigation:
```html
<a href="#services">Services</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact Us</a>
```

To update:
1. Replace `#services` with your actual URL
2. Example: `<a href="https://example.com/services">Services</a>`
3. For internal pages, use relative paths: `<a href="/services.html">Services</a>`

### Social Media Links
Located in the footer:
```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-400 hover:text-white">
        <i class="fab fa-facebook"></i>
    </a>
    <!-- Replace # with actual social media URLs -->
</div>
```

### Contact Information
Update email address:
```html
<a href="mailto:info@cupertinojunkremoval.com">
    Get Started Now
</a>
```

## Adding Privacy and Terms Pages

### Step 1: Add Footer Links
Insert this code in the footer's Quick Links section:
```html
<ul class="space-y-2">
    <li><a href="/privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="/terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
</ul>
```

### Step 2: Create New Pages
1. Create `privacy.html` and `terms.html` in your root directory
2. Copy the header and footer from `index.html`
3. Add your policy content between them

## Troubleshooting

### Common Issues

1. **Broken Links**
   - Check for typos in `href` attributes
   - Ensure file paths are correct
   - Test all links after updating

2. **Styling Problems**
   - Verify Tailwind CSS classes are spelled correctly
   - Check for missing closing tags
   - Maintain the responsive design classes (`md:`, `lg:` prefixes)

3. **Icon Issues**
   - Ensure Font Awesome is properly loaded
   - Check icon class names against [Font Awesome documentation](https://fontawesome.com/icons)

### Best Practices

1. Always backup files before making changes
2. Test changes on mobile and desktop views
3. Validate HTML at [W3C Validator](https://validator.w3.org/)
4. Keep consistent spacing and indentation

Need help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).