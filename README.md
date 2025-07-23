# Modern Design System

A comprehensive design token system with dark colors and blue/purple accents, featuring modern typography with thin font weights, reusable component styles, and beautiful animations.

![Design System Hero](https://img.shields.io/badge/Design_System-Modern_Dark_Theme-4F46E5?style=for-the-badge&logo=css3&logoColor=white)

## ✨ Features

- 🎨 **Dark Theme Optimized** - Rich dark backgrounds with carefully crafted blue/purple accents
- 🔤 **Modern Typography** - Inter font with emphasis on thin and light weights (100-600)
- 📱 **Responsive Design** - Fluid typography and spacing using CSS clamp()
- 🎭 **Component Library** - Complete set of reusable UI components
- 🌊 **Animation System** - Smooth transitions, hover effects, and scroll-triggered animations
- 🧩 **Design Tokens** - Systematic approach to colors, spacing, typography, and shadows
- ♿ **Accessibility** - Reduced motion support and proper contrast ratios
- ⚡ **Performance** - GPU-accelerated animations and optimized CSS

## 🚀 Quick Start

### Installation

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/design-system.git
cd design-system
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and visit `http://localhost:3000`

### Using in Your Project

Include the CSS files in your HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <link rel="stylesheet" href="tokens.css">
  <link rel="stylesheet" href="components.css">
  <link rel="stylesheet" href="animations.css">
</head>
<body>
  <!-- Your content here -->
</body>
</html>
```

## 🎨 Design Tokens

### Color System

Our design system is built on a dark theme foundation with blue/purple accents:

```css
/* Primary Accents */
--color-accent-primary: #4F46E5;    /* Indigo */
--color-accent-secondary: #7C3AED;  /* Violet */
--color-accent-tertiary: #06B6D4;   /* Cyan */

/* Dark Backgrounds */
--color-bg-primary: #0a0a0b;
--color-bg-secondary: #151518;
--color-bg-elevated: #242429;

/* Gradients */
--gradient-primary: linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%);
--gradient-secondary: linear-gradient(135deg, #06B6D4 0%, #4F46E5 100%);
```

### Typography

Modern typography system using Inter font:

```css
/* Font Weights - Emphasis on thin/light */
--font-weight-thin: 100;
--font-weight-light: 300;
--font-weight-normal: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;

/* Fluid Typography */
--font-size-5xl: clamp(3rem, 2.4rem + 3vw, 6rem);
--font-size-3xl: clamp(1.875rem, 1.5rem + 1.875vw, 3rem);
--font-size-xl: clamp(1.25rem, 1.1rem + 0.75vw, 1.5rem);
```

### Spacing System

8px-based spacing system for consistent layouts:

```css
--space-1: 0.25rem;   /* 4px */
--space-2: 0.5rem;    /* 8px */
--space-4: 1rem;      /* 16px */
--space-6: 1.5rem;    /* 24px */
--space-8: 2rem;      /* 32px */
```

## 🧩 Components

### Buttons

Multiple button variants with hover effects:

```html
<!-- Primary Button -->
<button class="btn btn-primary hover-lift">Primary Action</button>

<!-- Secondary Button -->
<button class="btn btn-secondary hover-scale">Secondary Action</button>

<!-- Ghost Button -->
<button class="btn btn-ghost">Subtle Action</button>

<!-- Accent Button -->
<button class="btn btn-accent hover-glow">Accent Action</button>
```

### Cards

Flexible card components for content display:

```html
<!-- Basic Card -->
<div class="card hover-lift">
  <div class="card-header">
    <h3 class="text-lg text-medium">Card Title</h3>
  </div>
  <div class="card-body">
    <p class="text-secondary">Card content goes here.</p>
  </div>
</div>

<!-- Elevated Card -->
<div class="card card-elevated">
  <div class="card-body">
    <h3 class="text-lg text-medium">Elevated Card</h3>
    <p class="text-secondary">Enhanced shadow and prominence.</p>
  </div>
</div>
```

### Tables

Comprehensive table system with multiple variants:

```html
<!-- Basic Table -->
<div class="table-container">
  <table class="table">
    <thead>
      <tr>
        <th class="table-sort">Name</th>
        <th class="table-cell-center">Status</th>
        <th class="table-cell-actions">Actions</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>John Doe</td>
        <td class="table-cell-center">
          <span class="table-status table-status-active">Active</span>
        </td>
        <td class="table-cell-actions">
          <button class="table-action-btn primary">Edit</button>
        </td>
      </tr>
    </tbody>
  </table>
</div>

<!-- Responsive Table -->
<div class="table-container table-responsive">
  <table class="table">
    <tbody>
      <tr>
        <td data-label="Name">John Doe</td>
        <td data-label="Email">john@example.com</td>
      </tr>
    </tbody>
  </table>
</div>
```

### Forms

Modern form inputs with focus states:

```html
<!-- Input Fields -->
<input type="text" class="input" placeholder="Default input">
<input type="text" class="input input-lg" placeholder="Large input">
<input type="text" class="input input-sm" placeholder="Small input">

<!-- Form Example -->
<form class="space-y-4">
  <div>
    <label class="text-sm text-secondary">Name</label>
    <input type="text" class="input" placeholder="Enter your name">
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```

### Badges & Status

Color-coded badges for status indication:

```html
<span class="badge badge-primary">Primary</span>
<span class="badge badge-success">Success</span>
<span class="badge badge-warning">Warning</span>
<span class="badge badge-error">Error</span>

<!-- Table Status Indicators -->
<span class="table-status table-status-active">Active</span>
<span class="table-status table-status-pending">Pending</span>
<span class="table-status table-status-error">Error</span>
```

## 🎭 Animations

### Fade Animations

```html
<!-- Basic Fade In -->
<div class="animate-fade-in">Fades in on load</div>

<!-- Fade In Up (for hero sections) -->
<div class="hero-title animate-fade-in-up">Hero Title</div>

<!-- Staggered Animations -->
<div class="animate-fade-in animate-delay-200">Delayed fade</div>
<div class="animate-fade-in animate-delay-500">More delayed</div>
```

### Hover Effects

```html
<!-- Lift Effect -->
<div class="card hover-lift">Lifts on hover</div>

<!-- Scale Effect -->
<button class="btn hover-scale">Scales on hover</button>

<!-- Glow Effect -->
<button class="btn btn-primary hover-glow">Glows on hover</button>
```

### Scroll Animations

```html
<!-- Fade in when scrolled into view -->
<div class="scroll-fade-in">Animates on scroll</div>
<div class="scroll-slide-left">Slides from left</div>
<div class="scroll-scale-in">Scales in on scroll</div>
```

## 📱 Responsive Design

The design system is built mobile-first with responsive breakpoints:

- **xs**: 400px (custom breakpoint)
- **sm**: 640px
- **md**: 768px
- **lg**: 1024px
- **xl**: 1280px
- **2xl**: 1536px

Tables automatically stack on mobile devices using the `.table-responsive` class.

## 🛠️ Development

### Available Scripts

```bash
# Start development server (Python HTTP server on port 3000)
npm run dev

# Start server on port 8080
npm run serve

# Alternative start command
npm start

# Build (static files ready for deployment)
npm run build
```

### File Structure

```
├── index.html          # Reference page with Hero section
├── tokens.css          # Design tokens (colors, typography, spacing)
├── components.css      # Component library
├── animations.css      # Animation system
├── package.json        # Project configuration
├── CLAUDE.md          # AI development guidance
└── README.md          # This file
```

### Adding New Components

1. Define component styles in `components.css`
2. Use existing design tokens from `tokens.css`
3. Add hover/animation effects from `animations.css`
4. Include examples in `index.html`

Example component:

```css
.my-component {
  padding: var(--space-4);
  color: var(--color-text-primary);
  background-color: var(--color-bg-secondary);
  border: 1px solid var(--color-border-primary);
  border-radius: var(--radius-md);
  transition: all var(--duration-normal) var(--ease-out);
}

.my-component:hover {
  background-color: var(--color-bg-elevated);
  transform: translateY(-1px);
}
```

## 🎯 Usage Examples

### Building a Dashboard

```html
<div class="container">
  <!-- Header -->
  <header class="flex justify-between items-center mb-8">
    <h1 class="text-3xl text-light">Dashboard</h1>
    <button class="btn btn-primary">New Item</button>
  </header>

  <!-- Stats Cards -->
  <div class="grid gap-6 mb-8" style="grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));">
    <div class="card p-6">
      <h3 class="text-lg text-medium mb-2">Total Users</h3>
      <p class="text-3xl text-accent">12,340</p>
    </div>
    <div class="card p-6">
      <h3 class="text-lg text-medium mb-2">Revenue</h3>
      <p class="text-3xl text-accent">$45,210</p>
    </div>
  </div>

  <!-- Data Table -->
  <div class="table-container">
    <table class="table">
      <thead>
        <tr>
          <th>User</th>
          <th class="table-cell-center">Status</th>
          <th class="table-cell-actions">Actions</th>
        </tr>
      </thead>
      <tbody>
        <!-- Table rows... -->
      </tbody>
    </table>
  </div>
</div>
```

### Creating a Landing Page

```html
<!-- Hero Section -->
<section class="hero-section" style="min-height: 100vh; display: flex; align-items: center;">
  <div class="container text-center">
    <h1 class="hero-title text-5xl text-thin mb-6">
      Beautiful Product Name
    </h1>
    <p class="hero-subtitle text-xl text-secondary mb-8">
      Elegant description of your amazing product.
    </p>
    <div class="hero-cta flex gap-4 justify-center">
      <button class="btn btn-primary btn-lg hover-lift">Get Started</button>
      <button class="btn btn-ghost btn-lg hover-scale">Learn More</button>
    </div>
  </div>
</section>
```

## 🎨 Customization

### Custom Colors

To add your own brand colors, extend the token system:

```css
:root {
  /* Add your brand colors */
  --color-brand-primary: #your-color;
  --color-brand-secondary: #your-color;
  
  /* Create custom gradients */
  --gradient-brand: linear-gradient(135deg, var(--color-brand-primary) 0%, var(--color-brand-secondary) 100%);
}

/* Use in components */
.btn-brand {
  background: var(--gradient-brand);
  color: var(--color-text-primary);
}
```

### Custom Components

Follow the established patterns:

```css
.custom-component {
  /* Use design tokens */
  padding: var(--space-4) var(--space-6);
  background-color: var(--color-bg-secondary);
  border-radius: var(--radius-lg);
  
  /* Add consistent transitions */
  transition: all var(--duration-normal) var(--ease-out);
  
  /* Include hover states */
}

.custom-component:hover {
  transform: translateY(-1px);
  box-shadow: var(--shadow-lg);
}
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/new-component`
3. Make your changes following the established patterns
4. Test your changes with `npm run dev`
5. Commit your changes: `git commit -m 'Add new component'`
6. Push to the branch: `git push origin feature/new-component`
7. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **Inter Font** - Beautiful modern typeface by Rasmus Andersson
- **Claude Code** - AI assistant for development
- **CSS Custom Properties** - For flexible design token system
- **Modern CSS** - Grid, Flexbox, and clamp() for responsive design

---

Built with ❤️ for modern web applications. Perfect for dashboards, admin panels, marketing sites, and any application requiring a professional dark theme aesthetic.

## 🔗 Links

- **Live Demo**: [View the design system](https://your-username.github.io/design-system)
- **Documentation**: See `CLAUDE.md` for development guidance
- **Issues**: Report bugs and feature requests
- **Discussions**: Share ideas and get help

---

*This design system was created to provide a solid foundation for modern web applications with a focus on dark themes, accessibility, and beautiful user experiences.*