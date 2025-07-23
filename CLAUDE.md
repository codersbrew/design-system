# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a comprehensive design token system with dark colors and blue/purple accents. It features modern typography with thin font weights, reusable component styles, and a complete reference HTML page with animations.

## Development Commands

```bash
# Start development server on port 3000
npm run dev

# Start server on port 8080
npm run serve

# Alternative start command
npm start

# Build (static files are ready for deployment)
npm run build

# Test (currently not implemented)
npm test
```

## Project Structure

```
├── index.html          # Main reference page with Hero section
├── tokens.css           # Design tokens (colors, typography, spacing)
├── components.css       # Reusable component styles
├── animations.css       # Animation system with motion effects
├── package.json         # Project configuration
└── CLAUDE.md           # This documentation file
```

## Design System Architecture

### Design Tokens (`tokens.css`)
- **Color System**: Dark theme with blue/purple accents (`--color-accent-primary`, `--color-accent-secondary`, `--color-accent-tertiary`)
- **Typography**: Modern Inter font with thin weights (100-600), fluid responsive sizing
- **Spacing**: 8px-based spacing system (`--space-1` through `--space-32`)
- **Gradients**: Primary, secondary, and subtle gradient combinations
- **Shadows**: Dark-optimized shadow system with accent variants

### Components (`components.css`)
- **Buttons**: Primary, secondary, ghost, and accent variants with hover effects
- **Cards**: Basic, elevated, and structured cards with headers/footers
- **Forms**: Input fields with focus states and validation styles
- **Navigation**: Modern nav links with active states
- **Badges & Status**: Color-coded badges and progress bars
- **Avatars**: Multiple sizes with gradient backgrounds
- **Modals & Tooltips**: Overlay components with backdrop blur

### Animations (`animations.css`)
- **Fade Effects**: FadeIn, FadeInUp, FadeInDown animations
- **Scale Effects**: ScaleIn and ScaleInUp for modal-style entrances
- **Hover Effects**: Lift, scale, glow, and rotate on hover
- **Scroll Triggers**: Elements animate when scrolling into view
- **Hero Animations**: Staggered text animations for landing sections

## Key Features

- **Responsive Design**: Fluid typography and spacing using clamp()
- **Dark Theme Optimized**: All colors and shadows designed for dark backgrounds
- **Modern Typography**: Inter font with emphasis on thin/light weights
- **Accessibility**: Reduced motion support, proper contrast ratios
- **Performance**: GPU-accelerated animations, optimized selectors

## Usage Patterns

### Using Design Tokens
```html
<div style="color: var(--color-accent-primary); padding: var(--space-6);">
```

### Component Classes
```html
<button class="btn btn-primary hover-lift">Click me</button>
<div class="card card-elevated p-6">Content</div>
```

### Animation Classes
```html
<div class="scroll-fade-in animate-delay-300">Animated content</div>
```

## Development Context

- **Framework**: Pure CSS with design tokens
- **Project Type**: Component-based design system
- **Status**: Complete reference implementation
- **Server**: Python HTTP server for development