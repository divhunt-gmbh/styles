# DH CSS Framework

A comprehensive, utility-first CSS framework with a complete dark theme design system. Built for modern web applications with consistent naming conventions and extensive utility coverage.

## 🚀 Features

- **Utility-first architecture** - Compose interfaces from small, single-purpose classes
- **Dark theme optimized** - Complete dark UI design system with opacity variants
- **Consistent naming** - Predictable `dh-` prefixed class names across all utilities
- **Minimal footprint** - Essential utilities without bloat
- **Custom properties** - Easy theming with CSS variables
- **Complete coverage** - Layout, spacing, typography, colors, effects, and more
- **Responsive ready** - Mobile-first responsive utilities
- **Modern CSS** - Uses latest CSS features for optimal performance

## 📦 Installation

### File Structure
```
/lib/styles/
├── classes/
│   ├── animations.css      # Fade, slide animations
│   ├── background.css      # Background colors & hover states
│   ├── border.css         # Borders, colors, radius
│   ├── color.css          # Text colors
│   ├── effects.css        # Shadows, transitions, opacity
│   ├── height.css         # Fixed height utilities
│   ├── interactivity.css  # Cursors, selections, hover states
│   ├── layout.css         # Flexbox, grid, display
│   ├── sizing.css         # Width, height, min/max sizes
│   ├── spacing.css        # Padding, margin, gap
│   ├── typography.css     # Fonts, sizes, weights, alignment
│   └── utility.css        # Text utilities, accessibility
├── main.css               # Combined imports
├── queries.css            # Responsive breakpoints
├── reset.css             # Base styles & normalization
└── variables.css         # CSS custom properties
```

### Import Methods
```css
/* Option 1: Import main stylesheet */
@import url('lib/styles/main.css');

/* Option 2: Import individual modules */
@import url('lib/styles/variables.css');
@import url('lib/styles/reset.css');
@import url('lib/styles/classes/layout.css');
/* ... other modules as needed */
```

## 🎨 Complete Design System

### 📏 Spacing Scale
| Variable | Value | Usage |
|----------|-------|-------|
| `--dh-spacing-x` | `4px` | Extra small - borders, fine details |
| `--dh-spacing-s` | `8px` | Small - compact spacing |
| `--dh-spacing-m` | `16px` | Medium - standard spacing |
| `--dh-spacing-l` | `24px` | Large - generous spacing |

**Classes:** `dh-p-{size}`, `dh-m-{size}`, `dh-px-{size}`, `dh-py-{size}`, `dh-pt-{size}`, `dh-pr-{size}`, `dh-pb-{size}`, `dh-pl-{size}`, `dh-gap-{size}`

### 🎨 Complete Color Palette

#### Background Colors
| Variable | Hex | Description | Border | Hover |
|----------|-----|-------------|--------|-------|
| `--dh-bg-1` | `#151515` | Darkest - main backgrounds | `#252525` | `#171717` |
| `--dh-bg-2` | `#1d1d1d` | Dark - cards, panels | `#2e2e2e` | `#1f1f1f` |
| `--dh-bg-3` | `#222222` | Medium - elevated surfaces | `#333333` | `#242424` |
| `--dh-bg-4` | `#272727` | Light - input fields, buttons | `#383838` | `#292929` |

**Classes:** `dh-bg-{1-4}`, `dh-hover-bg-{1-4}`, `dh-border-{1-4}`

#### Text Colors
| Variable | Hex | Usage |
|----------|-----|-------|
| `--dh-text-1` | `#FFFFFF` | Primary text, headings |
| `--dh-text-2` | `#b2b2b2` | Secondary text, descriptions |

**Classes:** `dh-text-{1-2}`, `dh-hover-text-{1-2}`

#### Brand & Semantic Colors
| Color | Base | Border | Opacity | Hover | Usage |
|-------|------|--------|---------|-------|-------|
| **Brand** | `#7F54F5` | `#9A77FF` | `rgba(127, 84, 245, 0.85)` | `#6A41E0` | Primary actions, links |
| **Blue** | `#0077FF` | `#3399FF` | `rgba(0, 119, 255, 0.85)` | `#005BDF` | Information, links |
| **Red** | `#FF0000` | `#FF3333` | `rgba(255, 0, 0, 0.85)` | `#CC0000` | Errors, danger |
| **Orange** | `#FF6D00` | `#FF8833` | `rgba(255, 109, 0, 0.85)` | `#CC5700` | Warnings, alerts |
| **Green** | `#00CC66` | `#33DD88` | `rgba(0, 204, 102, 0.85)` | `#00A352` | Success, positive |

**Classes:** `dh-bg-{color}`, `dh-text-{color}`, `dh-border-{color}`, `dh-hover-bg-{color}`, `dh-hover-text-{color}`

### 📝 Typography System

#### Font Families
```css
--dh-font-primary: 'Outfit'    /* Body text */
--dh-font-secondary: 'Outfit'  /* Headings */
```

#### Font Sizes
| Variable | Value | Usage |
|----------|-------|-------|
| `--dh-size-s` | `13px` | Small text, captions |
| `--dh-size-m` | `16px` | Body text, default |
| `--dh-size-l` | `22px` | Large text, emphasis |

#### Font Weights
- `dh-font-thin` (100)
- `dh-font-light` (300)  
- `dh-font-normal` (400)
- `dh-font-medium` (500)
- `dh-font-semibold` (600)
- `dh-font-bold` (700)
- `dh-font-black` (900)

#### Text Alignment
- `dh-text-left`
- `dh-text-center`
- `dh-text-right`
- `dh-text-justify`

#### Text Transform
- `dh-uppercase`
- `dh-lowercase`
- `dh-capitalize`
- `dh-normal-case`

#### Text Decoration
- `dh-underline`
- `dh-line-through`
- `dh-no-underline`

#### Line Heights
- `dh-leading-none` (1)
- `dh-leading-tight` (1.25)
- `dh-leading-snug` (1.375)
- `dh-leading-normal` (1.5)
- `dh-leading-relaxed` (1.625)
- `dh-leading-loose` (2)

### 📐 Border Radius
| Variable | Value | Usage |
|----------|-------|-------|
| `--dh-radius-s` | `4px` | Small - buttons, inputs |
| `--dh-radius-m` | `8px` | Medium - cards, panels |
| `--dh-radius-l` | `12px` | Large - modals, containers |

**Classes:** `dh-rounded-none`, `dh-rounded-s`, `dh-rounded-m`, `dh-rounded-l`, `dh-rounded-full`

### 📏 Height Scale
| Variable | Value | Usage |
|----------|-------|-------|
| `--dh-height-x` | `18px` | Extra small - thin bars |
| `--dh-height-s` | `24px` | Small - compact buttons |
| `--dh-height-m` | `34px` | Medium - standard inputs |
| `--dh-height-l` | `44px` | Large - prominent buttons |

**Classes:** `dh-height-{size}`, `dh-h-{size}`

## 🏗️ Layout System

### Flexbox Utilities
```html
<!-- Basic flex -->
<div class="dh-flex dh-flex-col">
<div class="dh-inline-flex">

<!-- Direction -->
<div class="dh-flex-row">    <!-- Default -->
<div class="dh-flex-col">    <!-- Column -->

<!-- Wrap -->
<div class="dh-flex-wrap">
<div class="dh-flex-nowrap">

<!-- Align items -->
<div class="dh-items-start">
<div class="dh-items-center">
<div class="dh-items-end">
<div class="dh-items-stretch">
<div class="dh-items-baseline">

<!-- Justify content -->
<div class="dh-justify-start">
<div class="dh-justify-center">
<div class="dh-justify-end">
<div class="dh-justify-between">
<div class="dh-justify-around">
<div class="dh-justify-evenly">

<!-- Flex grow/shrink -->
<div class="dh-flex-1">        <!-- flex: 1 1 0% -->
<div class="dh-flex-auto">     <!-- flex: 1 1 auto -->
<div class="dh-flex-none">     <!-- flex: none -->
<div class="dh-flex-grow">
<div class="dh-flex-grow-0">
<div class="dh-flex-shrink">
<div class="dh-flex-shrink-0">
```

### Flex Shortcuts
```html
<div class="dh-flex-center">      <!-- Centered content -->
<div class="dh-flex-between">     <!-- Space between -->
<div class="dh-flex-around">      <!-- Space around -->
<div class="dh-flex-start">       <!-- Align start -->
<div class="dh-flex-end">         <!-- Align end -->
<div class="dh-flex-col-center">  <!-- Column centered -->
<div class="dh-flex-col-start">   <!-- Column start -->
```

### Grid System
```html
<!-- Fixed columns -->
<div class="dh-grid-1">   <!-- 1 column -->
<div class="dh-grid-2">   <!-- 2 columns -->
<div class="dh-grid-3">   <!-- 3 columns -->
<div class="dh-grid-4">   <!-- 4 columns -->
<div class="dh-grid-5">   <!-- 5 columns -->
<div class="dh-grid-6">   <!-- 6 columns -->
<div class="dh-grid-8">   <!-- 8 columns -->
<div class="dh-grid-12">  <!-- 12 columns -->

<!-- Auto-fit responsive -->
<div class="dh-grid-auto">    <!-- min 200px -->
<div class="dh-grid-auto-s">  <!-- min 150px -->
<div class="dh-grid-auto-m">  <!-- min 250px -->
<div class="dh-grid-auto-l">  <!-- min 300px -->

<!-- Auto-fill responsive -->
<div class="dh-grid-fill">    <!-- min 200px -->
<div class="dh-grid-fill-s">  <!-- min 150px -->
<div class="dh-grid-fill-m">  <!-- min 250px -->
<div class="dh-grid-fill-l">  <!-- min 300px -->
```

### Grid Item Positioning
```html
<!-- Column span -->
<div class="dh-col-span-1">     <!-- Span 1 column -->
<div class="dh-col-span-2">     <!-- Span 2 columns -->
<!-- ... up to dh-col-span-12 -->
<div class="dh-col-span-full">  <!-- Span all columns -->

<!-- Row span -->
<div class="dh-row-span-1">     <!-- Span 1 row -->
<div class="dh-row-span-2">     <!-- Span 2 rows -->
<div class="dh-row-span-3">     <!-- Span 3 rows -->
<div class="dh-row-span-4">     <!-- Span 4 rows -->
<div class="dh-row-span-full">  <!-- Span all rows -->

<!-- Column start/end -->
<div class="dh-col-start-1">    <!-- Start at column 1 -->
<div class="dh-col-start-2">    <!-- Start at column 2 -->
<div class="dh-col-end-3">      <!-- End at column 3 -->
<div class="dh-col-end-auto">   <!-- Auto end -->
```

### Grid Alignment
```html
<!-- Place items -->
<div class="dh-place-items-start">
<div class="dh-place-items-center">
<div class="dh-place-items-end">
<div class="dh-place-items-stretch">

<!-- Place content -->
<div class="dh-place-content-start">
<div class="dh-place-content-center">
<div class="dh-place-content-end">
<div class="dh-place-content-between">
<div class="dh-place-content-around">
<div class="dh-place-content-evenly">

<!-- Place self -->
<div class="dh-place-self-start">
<div class="dh-place-self-center">
<div class="dh-place-self-end">
<div class="dh-place-self-stretch">
```

## 📱 Sizing System

### Width Utilities
```html
<div class="dh-w-auto">     <!-- width: auto -->
<div class="dh-w-full">     <!-- width: 100% -->
<div class="dh-w-fit">      <!-- width: fit-content -->
<div class="dh-w-min">      <!-- width: min-content -->
<div class="dh-w-max">      <!-- width: max-content -->
```

### Height Utilities
```html
<div class="dh-h-auto">     <!-- height: auto -->
<div class="dh-h-full">     <!-- height: 100% -->
<div class="dh-h-screen">   <!-- height: 100vh -->
<div class="dh-h-fit">      <!-- height: fit-content -->

<!-- Fixed heights -->
<div class="dh-h-x">        <!-- 18px -->
<div class="dh-h-s">        <!-- 24px -->
<div class="dh-h-m">        <!-- 34px -->
<div class="dh-h-l">        <!-- 44px -->
```

### Min/Max Sizes
```html
<!-- Min heights -->
<div class="dh-min-h-0">
<div class="dh-min-h-full">
<div class="dh-min-h-screen">

<!-- Max heights -->
<div class="dh-max-h-full">
<div class="dh-max-h-screen">

<!-- Min widths -->
<div class="dh-min-w-0">
<div class="dh-min-w-full">

<!-- Max widths -->
<div class="dh-max-w-xs">    <!-- 20rem -->
<div class="dh-max-w-s">     <!-- 24rem -->
<div class="dh-max-w-m">     <!-- 28rem -->
<div class="dh-max-w-l">     <!-- 32rem -->
<div class="dh-max-w-xl">    <!-- 36rem -->
<div class="dh-max-w-2xl">   <!-- 42rem -->
<div class="dh-max-w-3xl">   <!-- 48rem -->
<div class="dh-max-w-4xl">   <!-- 56rem -->
<div class="dh-max-w-5xl">   <!-- 64rem -->
<div class="dh-max-w-full">  <!-- 100% -->
<div class="dh-max-w-none">  <!-- none -->
```

## ✨ Effects & Animations

### Shadows
```html
<div class="dh-shadow-s">    <!-- Small shadow -->
<div class="dh-shadow-m">    <!-- Medium shadow -->
<div class="dh-shadow-l">    <!-- Large shadow -->
<div class="dh-shadow-xl">   <!-- Extra large shadow -->
<div class="dh-shadow-none"> <!-- No shadow -->
```

### Opacity
```html
<div class="dh-opacity-0">    <!-- Invisible -->
<div class="dh-opacity-25">   <!-- 25% visible -->
<div class="dh-opacity-50">   <!-- 50% visible -->
<div class="dh-opacity-75">   <!-- 75% visible -->
<div class="dh-opacity-100">  <!-- Fully visible -->

<!-- Hover states -->
<div class="dh-hover-opacity-25">
<div class="dh-hover-opacity-50">
<div class="dh-hover-opacity-75">
<div class="dh-hover-opacity-100">
```

### Transitions
```html
<div class="dh-transition">      <!-- 0.15s ease -->
<div class="dh-transition-slow"> <!-- 0.3s ease -->
<div class="dh-transition-none"> <!-- No transition -->
```

### Animations
```html
<div class="dh-animate-fade-in">    <!-- Fade in -->
<div class="dh-animate-slide-up">   <!-- Slide up -->
<div class="dh-animate-slide-down"> <!-- Slide down -->
```

## 🖱️ Interactivity

### Cursors
```html
<div class="dh-cursor-auto">
<div class="dh-cursor-default">
<div class="dh-cursor-pointer">
<div class="dh-cursor-not-allowed">
```

### User Selection
```html
<div class="dh-select-none">  <!-- Prevent selection -->
<div class="dh-select-text">  <!-- Text selection -->
<div class="dh-select-all">   <!-- Select all on click -->
```

### Pointer Events
```html
<div class="dh-pointer-events-none"> <!-- No pointer events -->
<div class="dh-pointer-events-auto"> <!-- Normal pointer events -->
```

## 🛠️ Utility Classes

### Text Utilities
```html
<!-- Truncation -->
<p class="dh-truncate">Long text that gets truncated with ellipsis...</p>

<!-- Line clamping -->
<p class="dh-line-clamp-1">Text limited to 1 line</p>
<p class="dh-line-clamp-2">Text limited to 2 lines</p>
<p class="dh-line-clamp-3">Text limited to 3 lines</p>
<p class="dh-line-clamp-4">Text limited to 4 lines</p>
<p class="dh-line-clamp-5">Text limited to 5 lines</p>
<p class="dh-line-clamp-6">Text limited to 6 lines</p>

<!-- Word breaking -->
<p class="dh-break-normal">Normal word breaking</p>
<p class="dh-break-words">Break long words</p>
<p class="dh-break-all">Break all characters</p>

<!-- Whitespace -->
<p class="dh-whitespace-normal">Normal whitespace</p>
<p class="dh-whitespace-nowrap">No wrapping</p>
<p class="dh-whitespace-pre">Preserve whitespace</p>
<p class="dh-whitespace-pre-line">Preserve line breaks</p>
<p class="dh-whitespace-pre-wrap">Preserve whitespace and wrap</p>
```

### Accessibility
```html
<div class="dh-sr-only">Screen reader only content</div>
```

### Display
```html
<div class="dh-block">        <!-- display: block -->
<div class="dh-inline-block"> <!-- display: inline-block -->
<div class="dh-hidden">       <!-- display: none -->
```

## 📱 Responsive Breakpoints

```css
/* Mobile (up to 575px) */
@media (max-width: 575.98px) { /* Custom styles */ }

/* Small tablets (576px to 767px) */
@media (min-width: 576px) and (max-width: 767.98px) { /* Custom styles */ }

/* Tablets (768px to 991px) */
@media (min-width: 768px) and (max-width: 991.98px) { /* Custom styles */ }

/* Desktops (992px to 1199px) */
@media (min-width: 992px) and (max-width: 1199.98px) { /* Custom styles */ }

/* Large desktops (1200px to 1399px) */
@media (min-width: 1200px) and (max-width: 1399.98px) { /* Custom styles */ }

/* Extra large desktops (1400px+) */
@media (min-width: 1400px) { /* Custom styles */ }
```

## 🎯 Complete Usage Examples

### Card Component
```html
<div class="dh-bg-2 dh-border dh-border-2 dh-rounded-m dh-p-l dh-shadow-m dh-transition dh-hover-bg-3">
    <h3 class="dh-text-1 dh-font-semibold dh-text-l dh-mb-s">Card Title</h3>
    <p class="dh-text-2 dh-mb-m dh-leading-relaxed">Card description with proper spacing and typography.</p>
    <div class="dh-flex-between">
        <span class="dh-text-s dh-text-2">Status</span>
        <button class="dh-bg-brand dh-text-1 dh-px-m dh-py-x dh-rounded-s dh-hover-bg-brand dh-transition">
            Action
        </button>
    </div>
</div>
```

## ⚙️ Customization

### Override Variables
```css
:root {
    /* Customize spacing */
    --dh-spacing-m: 20px;
    --dh-spacing-l: 32px;
    
    /* Customize colors */
    --dh-brand: #8B5CF6;
    --dh-brand-hover: #7C3AED;
    --dh-bg-1: #0F0F0F;
    
    /* Customize typography */
    --dh-font-primary: 'Inter', system-ui, sans-serif;
    --dh-size-m: 15px;
    
    /* Customize radius */
    --dh-radius-m: 6px;
    --dh-radius-l: 10px;
}
```

## 🌐 Browser Support

- **Chrome** 88+
- **Firefox** 85+  
- **Safari** 14+
- **Edge** 88+

## 📋 Checklist

### ✅ Complete Utility Coverage
- [x] **Layout** - Flexbox, Grid, Display
- [x] **Spacing** - Padding, Margin, Gap (all directions)
- [x] **Typography** - Fonts, Sizes, Weights, Alignment, Transform
- [x] **Colors** - Backgrounds, Text, Borders (all semantic colors)
- [x] **Sizing** - Width, Height, Min/Max dimensions
- [x] **Effects** - Shadows, Opacity, Transitions, Animations
- [x] **Borders** - Width, Colors, Radius
- [x] **Interactivity** - Cursors, Selection, Hover states
- [x] **Utilities** - Truncation, Line clamping, Accessibility
- [x] **Responsive** - Mobile-first breakpoints

### ✅ Design System Features
- [x] **Consistent naming** - `dh-` prefix throughout
- [x] **Dark theme optimized** - Complete dark color palette
- [x] **CSS Variables** - Fully customizable design tokens
- [x] **Hover states** - Interactive feedback for all colors
- [x] **Opacity variants** - Semi-transparent overlays
- [x] **Border variants** - Matching borders for all backgrounds

## 📄 License

MIT License - Free for personal and commercial use.

---

**DH CSS Framework** - A complete utility-first solution for modern dark theme applications.