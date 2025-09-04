# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Spanish-language landing page for "Booking Pro", an AI-powered WhatsApp appointment booking service. It's built as a single-page application using Vite, Tailwind CSS v4, and vanilla HTML/CSS/JavaScript.

## Development Commands

- `npm run dev` - Start development server (typically on port 3000 or next available)
- `npm run build` - Build production bundle 
- `npm run preview` - Preview production build locally

## Architecture & Technology Stack

### Core Technologies
- **Vite**: Build tool and dev server
- **Tailwind CSS v4**: Utility-first CSS framework with modern features
- **Inter Font**: Typography via Google Fonts and Inter CSS
- **Vanilla JavaScript**: No framework, just native DOM manipulation

### Project Structure
- `index.html` - Main HTML file with complete landing page
- `src/main.css` - Tailwind configuration and custom styles
- `vite.config.js` - Vite configuration with Tailwind plugin

## Tailwind CSS v4 Implementation

This project uses Tailwind CSS v4 with modern features:

### Custom Theme Configuration
- Custom color palette defined in `@theme` block in `src/main.css`
- Custom color variables: `--color-primary`, `--color-secondary`, etc.
- Inter font configuration with font feature settings

### Custom Utilities
- `@utility btnprimary` - Primary button styling
- `@utility btnwhatsapp` - WhatsApp-specific button with gradient and hover effects

### Animation System
The project uses extensive custom animations defined with `@keyframes` and `@utility`:
- `animate-fade-in-up` - Elements appear from bottom with fade
- `animate-slide-in-left/right` - Horizontal sliding animations  
- `animate-zoom-in` - Scale-up entrance animation
- `animate-bounce-gentle` - Subtle bouncing effect
- `animate-pulse-glow` - Text glow effect using `drop-shadow` filters
- `animate-float` - Floating background effects
- `gradientShift` - Animated gradient color shifting

### Modern CSS Features
- Uses `drop-shadow()` filters for glow effects compatible with gradient text
- Backdrop blur effects (`backdrop-blur-md`)
- CSS gradients with `bg-gradient-to-*` utilities
- Mix blend modes for background effects

## Landing Page Structure

The page consists of several main sections:
1. **Hero Section** - Dark gradient background with animated title and feature highlights
2. **Problem/Solution Section** - Contrasting problem vs solution cards with visual effects
3. **Features Section** - Three-column grid of main features
4. **Demo Section** - Interactive WhatsApp chat simulation
5. **Final CTA Section** - Call-to-action with multiple buttons and footer

### Key Design Patterns
- **Gradient Backgrounds**: Extensive use of dark gradients (`from-gray-900 via-black to-gray-900`)
- **Glass Morphism**: Fixed navigation with backdrop blur and transparency
- **Animated Text**: Word-by-word animations with staggered delays
- **Card-based Layout**: Bordered cards with gradient backgrounds and shadow effects
- **Mobile-First**: Responsive grid layouts that collapse on mobile

### Interactive Elements
- Mobile hamburger menu with animated icons
- Hover effects on buttons and cards
- Animated background blur circles
- Sequential text animations with timing delays

## Styling Conventions

- **Animation Delays**: Use inline `style="animation-delay: Xs"` for sequential animations
- **Color Scheme**: Red for problems, green/blue for solutions, gradients for highlights
- **Typography**: Consistent use of font weights (extrabold for headings, medium/semibold for content)
- **Spacing**: Liberal use of padding and margins for breathing room
- **Effects**: Combine multiple visual effects (gradients, shadows, borders, blur) for depth

## Important Notes

- All text content is in Spanish
- Uses semantic color coding (red=problems, green=solutions)
- Heavy emphasis on visual effects and animations
- Single HTML file approach - all content is in `index.html`
- No external JavaScript frameworks, but includes vanilla JS for mobile menu functionality