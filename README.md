# Timeless Jewelry Landing Page - Maintenance Guide

This guide will help you maintain and customize the Timeless Jewelry landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## 1. Updating Text and Tailwind CSS Classes

### Header Section
```html
<!-- Original Header Text -->
<div class="text-2xl font-bold">Timeless</div>
```
To modify the company name:
1. Locate the header section at the top of the page
2. Change "Timeless" to your desired text
3. Adjust size using Tailwind classes:
   - `text-xl` (smaller)
   - `text-2xl` (current size)
   - `text-3xl` (larger)

### Hero Section Text
```html
<h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">
    Jewelry Timeless Elegance and Crafted
</h1>
<p class="text-xl md:text-2xl mb-8">Discover Your Perfect Piece</p>
```
To update hero content:
1. Replace heading text between `<h1>` tags
2. Modify subtitle between `<p>` tags
3. Keep responsive classes (`md:text-6xl`) to maintain mobile compatibility

### Tailwind CSS Class Guide
Common classes used throughout:
- Layout: `container`, `mx-auto`, `px-6`, `py-4`
- Spacing: `mb-6`, `mt-12`, `space-x-8`
- Colors: `bg-gray-900`, `text-white`, `hover:bg-gray-800`
- Typography: `text-2xl`, `font-bold`, `text-center`

⚠️ **Important**: Always maintain both mobile (`text-xl`) and desktop (`md:text-2xl`) sizes when modifying text classes.

## 2. Fixing Broken Links

### Navigation Menu Links
Current placeholder links:
```html
<a href="#" class="text-gray-700 hover:text-gray-900">Watches</a>
<a href="#" class="text-gray-700 hover:text-gray-900">Necklaces</a>
<a href="#" class="text-gray-700 hover:text-gray-900">Rings</a>
```

To update navigation links:
1. Replace `#` with proper URLs:
```html
<a href="/watches.html" class="text-gray-700 hover:text-gray-900">Watches</a>
```
2. Ensure URLs match your file structure
3. Test all links after updating

### Footer Quick Links
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white">About Us</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white">Collections</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white">Blog</a></li>
</ul>
```

To update footer links:
1. Replace `#` with corresponding page URLs
2. Maintain consistent styling classes
3. Add new links by copying existing `<li>` elements

### Social Media Links
```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-400 hover:text-white">
        <!-- Facebook SVG -->
    </a>
</div>
```

To update social links:
1. Replace `#` with full social media profile URLs
2. Keep SVG icons intact
3. Test hover effects after updating

## 3. Adding Privacy and Terms Pages

### Footer Modification
Add privacy and terms links to the Quick Links section:
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white">About Us</a></li>
    <!-- Add these new links -->
    <li><a href="/privacy.html" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
    <li><a href="/terms.html" class="text-gray-400 hover:text-white">Terms of Service</a></li>
</ul>
```

### Alternative Footer Layout
For a separate legal links section:
```html
<div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-400">
    <p>&copy; 2024 Timeless. All rights reserved.</p>
    <!-- Add this new div -->
    <div class="mt-4 space-x-4">
        <a href="/privacy.html" class="text-gray-400 hover:text-white">Privacy Policy</a>
        <a href="/terms.html" class="text-gray-400 hover:text-white">Terms of Service</a>
    </div>
</div>
```

## Troubleshooting Tips

1. **Broken Styles**
   - Check for typos in Tailwind class names
   - Ensure all classes are space-separated
   - Verify responsive classes start with `md:` or `lg:`

2. **Link Issues**
   - Confirm file paths match your directory structure
   - Use relative paths (`./` or `../`) for local files
   - Use full URLs for external links

3. **Mobile Display Problems**
   - Test using browser dev tools mobile view
   - Verify mobile menu functionality
   - Check responsive classes are properly set

## Need Help?

If you encounter issues:
1. Compare your changes with the original code
2. Check browser console for errors
3. Verify all files are in the correct locations
4. Test on multiple devices and browsers

Remember to always backup your code before making significant changes!