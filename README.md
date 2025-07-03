# Student Portfolio

## Overview

This repository contains a modern, responsive portfolio website. The application is built as a single-page application (SPA) using vanilla HTML, CSS, and JavaScript, featuring a clean design with dark/light theme switching capabilities and mobile-responsive navigation.

## System Architecture

### Frontend Architecture
- **Static Web Application**: Pure HTML/CSS/JavaScript implementation without any backend framework
- **Single Page Application**: All content is contained within a single HTML file with JavaScript-driven navigation
- **Responsive Design**: Mobile-first approach with responsive breakpoints
- **Theme System**: CSS custom properties-based theming with localStorage persistence

### Technology Stack
- **HTML5**: Semantic markup structure
- **CSS3**: Modern CSS with custom properties, flexbox, and grid layouts
- **Vanilla JavaScript**: No frameworks or libraries for core functionality
- **External Dependencies**: 
  - Google Fonts (Inter font family)
  - Font Awesome icons (CDN)

## Key Components

### 1. Navigation System
- **Responsive navbar** with hamburger menu for mobile devices
- **Smooth scrolling** navigation between sections
- **Theme toggle** button with icon switching
- **Mobile menu** with overlay functionality

### 2. Theme Management
- **Dual theme support** (light/dark modes)
- **CSS custom properties** for consistent theming
- **localStorage persistence** for user preference retention
- **Dynamic icon switching** based on active theme

### 3. User Interface Components
- **Hero section** with call-to-action buttons
- **Navigation menu** with section links
- **Responsive design** with mobile-first approach
- **Interactive elements** with hover states and transitions

### 4. Content Sections
- Home/Hero section
- About section
- Skills section
- Projects section
- Certifications section
- Contact section

## Data Flow

### Theme Management Flow
1. User clicks theme toggle button
2. JavaScript detects current theme from body attribute
3. Theme is switched and saved to localStorage
4. CSS custom properties update instantly
5. Theme icon updates to reflect new state

### Navigation Flow
1. User clicks navigation link or hamburger menu
2. JavaScript handles smooth scrolling to target section
3. Mobile menu closes automatically on link click
4. Active states update based on scroll position

## External Dependencies

### CDN Dependencies
- **Google Fonts**: Inter font family for typography
- **Font Awesome**: Icon library for UI elements (moon/sun icons, hamburger menu)

### Browser APIs
- **localStorage**: For theme preference persistence
- **DOM API**: For element manipulation and event handling
- **CSS Custom Properties**: For dynamic theming

## Deployment Strategy

### Static Hosting
- **Platform**: Suitable for any static hosting service (Netlify, Vercel, GitHub Pages)
- **Build Process**: No build process required - direct deployment of source files
- **Browser Support**: Modern browsers with CSS custom properties support
- **Performance**: Optimized for fast loading with minimal dependencies

### File Structure
```
/
├── index.html          # Main HTML file
├── styles.css          # CSS styles with theme system
├── script.js           # JavaScript functionality
└── replit.md          # Project documentation
```

## Changelog

```
Changelog:
- July 03, 2025. Initial setup
- July 03, 2025. Added Netflix-style horizontal scrolling navigation for projects and certifications
- July 03, 2025. Updated contact section with professional form layout
- July 03, 2025. Redesigned projects section with modern card layout and colored tech tags
- July 03, 2025. Added "Show More/Show Less" functionality for projects section
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```

## Development Notes

### Code Architecture Decisions

1. **Vanilla JavaScript Choice**: 
   - **Problem**: Need for lightweight, fast-loading portfolio
   - **Solution**: Pure JavaScript without frameworks
   - **Rationale**: Reduces bundle size, improves performance, and eliminates dependency management

2. **CSS Custom Properties for Theming**:
   - **Problem**: Need for consistent, maintainable theme switching
   - **Solution**: CSS custom properties with data attributes
   - **Rationale**: Provides instant theme switching without CSS file duplication

3. **Mobile-First Responsive Design**:
   - **Problem**: Portfolio needs to work on all devices
   - **Solution**: Mobile-first CSS with progressive enhancement
   - **Rationale**: Ensures optimal mobile experience and better performance

4. **localStorage for Theme Persistence**:
   - **Problem**: User theme preference should persist between sessions
   - **Solution**: Save theme choice to localStorage
   - **Rationale**: Improves user experience without requiring backend storage

### Future Enhancement Opportunities
- Add animation libraries for enhanced visual effects
- Implement intersection observer for scroll-triggered animations
- Add form handling for contact section
- Integrate with headless CMS for dynamic content management
