# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based personal academic website for AI researcher Arnaud Lallouet. The site uses the minimal Jekyll theme and consists of a multi-page structure with HTML files, CSS styling, and JavaScript for interactions.

## Architecture

### File Structure
- **HTML Pages**: Main content files (`index.html`, `about.html`, `publications.html`, `blog.html`, `contact.html`, individual blog posts)
- **Styling**: Single `styles.css` file containing all page styles with responsive design
- **JavaScript**: `script.js` handles navigation interactions, smooth scrolling, and animations
- **Configuration**: `_config.yml` contains Jekyll site configuration

### Design System
The site uses a consistent design language with:
- **Colors**: Primary blue (`#2563eb`), neutral grays for text, light backgrounds
- **Typography**: Inter font family with varying weights (300-600)
- **Layout**: CSS Grid and Flexbox for responsive layouts
- **Components**: Reusable card patterns, navigation, hero sections

### Page Structure
Each page follows a consistent pattern:
1. Fixed navigation header with transparent background and blur effect
2. Page-specific hero/header section
3. Main content area with consistent spacing (80px padding)
4. Footer with copyright information

## Development Commands

This is a static Jekyll site hosted on GitHub Pages. No package.json or build tools are present.

### Local Development
```bash
# Serve the site locally (requires Jekyll)
bundle exec jekyll serve

# Build the site
bundle exec jekyll build
```

### Deployment
The site is automatically deployed via GitHub Pages when changes are pushed to the main branch.

## Key Implementation Details

### Navigation
- Fixed header with backdrop blur effect
- Active page highlighting
- Smooth scroll behavior for anchor links
- Responsive collapse on mobile (CSS-only, no JS toggle implemented)

### Animations
- CSS-based fade-in animations using `@keyframes fadeInUp`
- Intersection Observer API for scroll-triggered animations
- Hover effects on cards and buttons

### Responsive Design
- Mobile-first approach with breakpoints at 768px and 480px
- Grid layouts that collapse to single columns on smaller screens
- Consistent spacing and typography scaling

### Content Areas
- **Home**: Hero section with profile placeholder, feature cards
- **About**: Bio section, research interests, education/experience placeholders
- **Publications**: Publication listings with filtering capabilities
- **Blog**: Blog post listings with sidebar, individual post pages
- **Contact**: Contact form, academic profile links, collaboration opportunities

## Style Conventions

- Use semantic HTML5 elements
- CSS follows a component-based approach with utility classes
- Consistent naming: kebab-case for CSS classes, camelCase for JavaScript
- Color variables should reference the established palette
- Maintain the existing grid systems and spacing units (rem-based)