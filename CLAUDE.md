# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website called "pohadkyprokluky.cz" (Fairy Tales for Boys) - a Czech children's storytelling website featuring bedtime stories specifically designed for boys who prefer cars, planes, trains, and machinery over traditional fairy tales.

## Architecture

### Site Structure
- **Static HTML website** with no build system or package management
- **Bootstrap-based layout** using CDN-hosted Bootstrap 5.2.3
- **Google Analytics integration** (gtag.js) for tracking
- **Simple file organization**:
  - `index.html` - Main landing page with story cards
  - Individual story pages (e.g., `pohadka-o-dvou-letadylkach.html`)
  - `css/styles.css` - Custom styles (minimal, mostly Bootstrap)
  - `js/scripts.js` - Currently empty placeholder
  - `assets/` - Images for stories and UI elements

### Content Pattern
Each story follows a consistent HTML structure:
- Bootstrap navbar with site branding
- Header section with story-specific imagery
- Main content area with the fairy tale text
- "Knowledge Corner" educational sections
- Footer with copyright

### Styling
- Uses Bootstrap 5 framework via CDN
- Custom CSS is minimal (Start Bootstrap Blog Home template)
- Responsive design with card-based layout
- Dark navbar with light content areas

## Development Workflow

### No Build Process
This is a static site with no build tools, package managers, or development dependencies. Files can be edited directly and viewed in a browser.

### Local Development
- Open `index.html` directly in a browser for testing
- Use a simple HTTP server if needed: `python -m http.server 8000`
- All dependencies are loaded via CDN

### Content Management
- Stories are individual HTML files following the established template
- Images are stored in `assets/` directory
- New stories require:
  1. Creating new HTML file following existing pattern
  2. Adding story card to `index.html`
  3. Adding appropriate images to `assets/`

### Deployment
- Static files can be deployed to any web server
- No build step required - deploy files as-is
- Ensure proper MIME types for static assets

## Key Considerations

- **Czech language content** - all text is in Czech
- **SEO optimized** with proper meta descriptions and structured content
- **Child-friendly themes** focusing on vehicles, machinery, and adventure
- **No external dependencies** beyond Bootstrap and Google Analytics CDN
- **Educational components** - each story includes "Knowledge Corner" sections