# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML website for "Project Freigeist" - a German blog/project showcasing creative work and philosophical content. The project consists of static HTML pages with CSS styling, focused on presenting content in both German and English.

## Architecture

The codebase is a simple static website with the following structure:

- **HTML Pages**: Multiple static HTML pages with semantic structure
  - `index.html` - Main English project showcase page
  - `projekt.html` - German version with blog-style layout and Jersey 25 font
  - `explanation.html` - Project explanation page
  - `resources.html` - Resources and links page
- **Styling**: Single CSS file (`styles.css`) with clean, minimalist design
- **No Build System**: This is a pure static site with no build process or dependencies

## Key Design Patterns

1. **Dual Language Support**: The site has both English (`index.html`, `explanation.html`, `resources.html`) and German (`projekt.html`) versions with different design approaches
2. **Typography**: German version uses Google Fonts (Jersey 25), English version uses serif fallbacks
3. **Layout**: Responsive grid-based layout with fixed header navigation
4. **Styling Approach**: External CSS file for English pages, inline styles for German page

## Development Workflow

Since this is a static HTML site:
- **Preview**: Open HTML files directly in browser or use a local HTTP server
- **No Build Process**: Changes to HTML/CSS are immediately visible
- **No Package Manager**: No npm, yarn, or other dependency management
- **No Testing Framework**: No automated tests configured

## Content Structure

- English pages follow a portfolio/showcase structure
- German page (`projekt.html`) follows a blog format with post listings
- Navigation is consistent between language versions but with different styling approaches
- Footer copyright notices are aligned with respective page languages

## Styling Guidelines

- English pages: Clean, minimalist design with serif typography
- German page: More expressive with custom font and retro-style borders
- Consistent color schemes within each language variant
- Responsive design considerations implemented for mobile devices