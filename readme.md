# Silky Looks - A Lightweight CSS Framework

Silky Looks is a modern, responsive CSS framework that uses custom HTML elements (components) to provide a clean and consistent design system. It features automatic dark/light theme support and a comprehensive set of layout and UI components.

## Installation
```css
@import url('https://silky-dot-dev.github.io/looks/good.css');
```

## Key Features

- **Custom HTML Elements**: Uses semantic custom elements with `s-` prefix (e.g., `s-card`, `s-container`, `s-grid`)
- **Automatic Theming**: Built-in support for light and dark themes using CSS `prefers-color-scheme`
- **Responsive Design**: Mobile-first approach with responsive breakpoints and adaptive layouts
- **Flexbox-based Layout System**: Modern CSS Grid and Flexbox for layouts
- **Zero JavaScript Required**: Pure CSS framework with optional JavaScript enhancements

## Components Available

### Layout Components
- `s-container` - Main content container with responsive padding
- `s-row` - Horizontal flex container with optional wrapping (`wrap`, `wrap-mobile` attributes)
- `s-column` - Vertical flex container with consistent spacing
- `s-grid` - CSS Grid container with configurable columns (2, 3, 4 columns via `columns` attribute)
- `s-spacer` - Flexible spacer element for pushing content apart

### UI Components
- `s-card` - Styled container with padding, border radius, and theme-aware background
- `s-appbar` - Fixed top navigation bar with built-in theming
- `s-toolbar` - Horizontal toolbar for buttons and actions
- `s-footer` - Fixed bottom footer component
- `s-badge` - Small label/badge component that can overlay buttons
- `s-notification` - Alert/notification component
- `s-gap` - Spacing utility component

### Utility Features
- `text="muted"` attribute for muted text styling
- `variant="outlined"` attribute for outlined button style
- `hide-on-mobile` / `hide-on-desktop` attributes for responsive visibility
- CSS custom properties for consistent spacing and theming

## Design System

### Spacing Scale
- `--spacing-s: 5px`
- `--spacing-m: 10px`
- `--spacing-l: 20px`

### Theme Variables
- Automatic light/dark theme switching based on user preference
- Consistent color palette across all components
- Theme-aware borders, backgrounds, and text colors

### Responsive Breakpoints
- Mobile: max-width 600px and 800px
- Desktop: min-width 801px
- Components automatically adapt layouts for different screen sizes

## Usage Examples

```html
<!-- Basic layout -->
<s-container>
  <s-row>
    <s-card>
      <h3>Card Title</h3>
      <p text="muted">Card content with muted text</p>
      <button>Primary Action</button>
      <button variant="outlined">Secondary Action</button>
    </s-card>
  </s-row>
</s-container>

<!-- Grid layout -->
<s-grid columns="3">
  <s-card>Grid Item 1</s-card>
  <s-card>Grid Item 2</s-card>
  <s-card>Grid Item 3</s-card>
</s-grid>

<!-- App structure -->
<s-appbar>
  <h2>App Title</h2>
  <s-toolbar>
    <button>Login</button>
  </s-toolbar>
</s-appbar>
```

## File Structure
- `good.css` - Main framework CSS file with all component styles and theming
- `index.html` - Demo page showcasing all components and features
- `logo.svg` - Framework logo/icon

## Browser Support
Modern browsers with CSS Grid, Flexbox, and CSS custom properties support. Designed for contemporary web development with clean, semantic markup.

This framework is ideal for rapid prototyping and building modern web applications with a consistent design system and minimal setup overhead.
