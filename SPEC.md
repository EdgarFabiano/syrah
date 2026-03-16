# Syrah Centro Clínico - Website Specification

## Project Overview
- **Project name**: Syrah Centro Clínico Website
- **Type**: Single-page medical clinic website
- **Core functionality**: Professional medical clinic website with service showcase, team presentation, contact/booking integration
- **Target users**: Patients seeking medical care, nutrition, and wellness services in Brasília/Águas Claras

## UI/UX Specification

### Layout Structure
- **Header**: Fixed navigation with logo and menu links
- **Hero**: Full-width section with headline, subheadline, CTAs
- **About**: Two-column layout with text and visual
- **Specialties**: Card grid layout
- **Differentials**: Feature boxes
- **Team**: Professional cards grid
- **Insurance**: Clean list/grid
- **Payment**: Icon row
- **Location**: Map and info
- **CTA Section**: Final conversion section
- **Footer**: Complete footer with links

### Responsive Breakpoints
- Mobile: < 768px (single column, stacked)
- Tablet: 768px - 1024px (2 columns)
- Desktop: > 1024px (full layout)

### Visual Design

#### Color Palette
- **Primary (Deep Green)**: #1f4d2b
- **Primary Dark**: #153a1f
- **Primary Light**: #2a6b3c
- **Gold Accent**: #c9a227
- **Gold Light**: #e8d48b
- **Background Light**: #f9faf8
- **Background Cream**: #f5f3ef
- **Text Dark**: #1a1a1a
- **Text Gray**: #5a5a5a
- **Text Light**: #ffffff
- **Border**: #e5e5e0

#### Typography
- **Headings**: "DM Sans" (sans-serif) - clean, modern, readable
- **Body**: "DM Sans" (sans-serif) - modern, clean, readable
- **Sizes**:
  - H1: 3.5rem (desktop), 2.5rem (mobile)
  - H2: 2.5rem (desktop), 2rem (mobile)
  - H3: 1.5rem
  - Body: 1rem
  - Small: 0.875rem

#### Spacing System
- Section padding: 100px vertical (desktop), 60px (mobile)
- Container max-width: 1200px
- Card padding: 30px
- Grid gap: 30px

#### Visual Effects
- Box shadows: 0 4px 30px rgba(31, 77, 43, 0.08)
- Hover transitions: 0.3s ease
- Border radius: 12px (cards), 8px (buttons), 50% (avatars)
- Subtle parallax on hero
- Fade-in animations on scroll

### Components

#### Header
- Logo (grape leaf icon + text)
- Navigation links (smooth scroll)
- Mobile hamburger menu

#### Buttons
- Primary: Green background, white text, gold hover
- Secondary: Transparent with green border

#### Cards
- White background
- Subtle shadow
- Hover lift effect
- Icon/animation on hover

#### Professional Cards
- Circular photo placeholder (placeholder gradient)
- Name in heading font
- Specialty in body font

## Functionality Specification

### Core Features
1. **Smooth Scrolling**: All navigation links scroll to sections
2. **Mobile Menu**: Hamburger toggle for mobile
3. **Scroll Animations**: Elements fade in on scroll
4. **Floating WhatsApp**: Fixed button bottom-right
5. **WhatsApp Integration**: Direct links to clinic WhatsApp
6. **Google Maps Link**: Opens map in new tab

### User Interactions
- Click nav link → smooth scroll to section
- Click WhatsApp → open wa.me link
- Hover on cards → subtle lift and shadow
- Scroll page → elements animate in

### SEO Requirements
- Semantic HTML5
- Meta tags
- Alt text placeholders
- Proper heading hierarchy

## Acceptance Criteria
- [x] All 10 sections implemented
- [x] Colors match brand spec
- [x] Typography uses DM Sans only
- [x] Responsive on all breakpoints
- [x] Smooth scrolling works
- [x] WhatsApp links work correctly
- [x] All content is in Portuguese
- [x] Floating WhatsApp button visible
- [x] Professional, premium medical aesthetic
- [x] Fast loading (no heavy assets)
