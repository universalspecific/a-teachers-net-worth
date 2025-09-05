# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a promotional website for the book "A Teacher's Net Worth" by Suzanne Zentner, Ph.D., MBA. The project consists of a single HTML file (`book-promo-site.html`) that creates a professional landing page for the book, which helps teachers build smart financial futures.

## Architecture

- **Single-file website**: The entire website is contained in one HTML file with embedded CSS and JavaScript
- **Static website**: No build process or server-side components
- **Responsive design**: Uses CSS Grid and Flexbox for mobile-friendly layouts
- **Embedded assets**: Book cover image is base64-encoded directly in the HTML

## Key Components

### HTML Structure
- Header with navigation
- Hero section with book cover and endorsement
- Story section explaining the book's origin
- Impact section highlighting benefits for educators, districts, and the profession
- Resources section listing what's included in the book
- Newsletter signup form
- Author bio section
- Footer with social links

### CSS Architecture
- CSS custom properties (variables) for consistent theming
- Mobile-first responsive design with media queries
- Component-based styling approach
- CSS Grid for layout, Flexbox for alignment

### JavaScript Features
- Smooth scrolling navigation
- Dynamic header background opacity on scroll
- Form handling for newsletter signup

## Development

### File Structure
```
/
├── book-promo-site.html    # Main website file
├── atnw-book-cover.jpg     # Book cover image (separate file)
├── financial-seminar.png   # Additional image asset
└── financial-teacher.jpg   # Additional image asset
```

### Making Changes
- Edit `book-promo-site.html` directly for content, styling, or functionality changes
- The book cover image is embedded as base64 in the HTML, but separate image files exist for reference
- No build process is required - changes are immediately visible when opening the HTML file

### Testing
Open `book-promo-site.html` directly in a web browser to test changes. No local server required.

### Deployment
The HTML file can be deployed to any static hosting service (GitHub Pages, Netlify, Vercel, etc.) as-is.

## External Integrations

- **Purchase links**: Amazon and IngramSpark links for book purchases
- **Newsletter form**: Uses Formspree (form action needs to be updated with actual form ID)
- **Social media**: Placeholder links for LinkedIn, Twitter/X, and email (need to be updated with actual URLs)

## Customization Notes

- Update social media links in the footer with actual URLs
- Replace Formspree form ID in newsletter signup
- Consider extracting base64 image to improve page load if needed
- Color scheme uses CSS variables for easy theme changes