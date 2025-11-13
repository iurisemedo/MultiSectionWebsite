# #1 FREE LEAKS - Model Showcase Website

## Overview
A high-conversion, single-page model showcase website built with Tailwind CSS, featuring a sleek Apple-inspired dark theme design with smooth animations and mobile-first responsive layout.

## Project Structure
```
.
├── index.html              # Complete single-file website (HTML, CSS, JS)
├── attached_assets/        # Model images and media files
└── replit.md              # This file
```

## Features

### Navigation Bar
- Fixed top navigation with dark theme
- "#1 FREE LEAKS" logo on the left
- "Join Discord" and "Join Telegram" CTA buttons on the right
- Smooth backdrop blur effect

### Hero Section
- Large, bold "#1 FREE LEAKS" heading in accent color (#87CEEB)
- "Best prices on the market" subheading
- Smooth fade-in and slide-up animations on scroll
- Compact layout for quick user engagement

### Premium Access Pack Section
- Dedicated section between hero and gallery
- Displays three pricing tiers in compact grid:
  - **Weekly**: €6.99/week
  - **Monthly**: €19.99/month (highlighted as "POPULAR")
  - **Lifetime**: €59.99 (one-time payment)
- Clear value proposition: "Unlock unlimited access to all models + custom requests"
- "Upgrade Now" button opens full premium modal
- Dark gradient backgrounds with accent highlights
- Responsive layout (stacks on mobile, grid on desktop)

### Model Gallery
- **30 model cards** displayed in a responsive grid
  - 2 columns on mobile
  - 3 columns on tablet
  - 4 columns on desktop
- **Real-time search functionality** - filters models as you type
- Each card includes:
  - High-quality model image (full display, no cropping with `object-contain`)
  - Model name only (clean, minimal design)
- Hover effects with elevation and shadow
- Scroll-triggered fade-in animations for each card
- Images display completely without cropping, using dark letterbox background for consistency

### Premium Upgrade Modal
- Full-screen overlay modal with 3 symmetrical pricing tiers:
  - **Weekly**: €6.99/week
  - **Monthly**: €19.99/month (highlighted as "POPULAR")
  - **Lifetime**: €59.99 (one-time payment)
- Perfect symmetry with aligned heights and centered content
- Features list:
  - Access to all models
  - Custom model requests
- Smooth animations when opening
- Close via X button, outside click, or Escape key

## Technical Implementation

### Design System
**Dark Theme Color Palette:**
- **Background**: #0F172A (dark slate)
- **Card/Surface**: #1E293B (lighter slate)
- **Primary Text**: #FFFFFF (white)
- **Secondary Text**: #D1D5DB / #9CA3AF (light gray)
- **Accent Color**: #87CEEB (light blue)
- **Borders**: #374151 (gray-700)

**Typography:**
- **Headings**: Poppins Bold
- **Body**: Inter (400, 500, 600 weights)

### Technology Stack
- **HTML5** - Semantic markup
- **Tailwind CSS** (CDN) - Utility-first styling
- **Vanilla JavaScript** - No framework dependencies
- **IntersectionObserver API** - Scroll animations

### Key JavaScript Features
1. **Search Filter**: Real-time filtering using `data-name` attributes
2. **Scroll Animations**: IntersectionObserver triggers fade-in/slide-up effects
3. **Modal Management**: Open/close with multiple interaction methods
4. **Smooth Scrolling**: CSS `scroll-behavior: smooth`

### Performance Optimizations
- Mobile-first responsive design
- Lazy-load scroll animations (elements animate only when visible)
- Optimized image loading
- Minimal JavaScript dependencies
- Single HTTP request for main page load

## Development Notes

### Current Setup
- Web server running on port 5000 (Python's http.server)
- Serves static HTML file with all assets
- No build process required - everything in single file

### Known Limitations
- TailwindCSS CDN used (suitable for development/demo)
  - For production, should install Tailwind as PostCSS plugin
- All code in single HTML file (as per requirements)
  - Makes development simpler but harder to maintain at scale

## Recent Changes
- November 13, 2025: Initial website creation
  - Created complete single-file HTML structure
  - Implemented 30 model cards with real images from attached_assets
  - Added functional search bar with real-time filtering
  - Implemented IntersectionObserver scroll animations
  - Created premium pricing modal with 3 tiers
  - Fixed image path issues for special character filenames
  - Configured workflow to serve on port 5000
  - **Converted entire design to dark theme** with Apple-inspired aesthetics
    - Updated all backgrounds to dark slate (#0F172A)
    - Updated cards and surfaces to lighter slate (#1E293B)
    - Adjusted all text colors for optimal contrast
    - Updated buttons, borders, and hover states
    - Modified pricing modal with dark gradients
    - Architect-reviewed and approved
  - **Updated image display to show full photos without cropping**
    - Changed from `object-cover` to `object-contain` 
    - Added dark letterbox background for consistent framing
    - All model images now display completely without cutting any parts

## Future Enhancements
- Add actual payment integration (Stripe/PayPal)
- Implement backend API for model data
- Add user authentication system
- Create admin panel for content management
- Implement Discord/Telegram bot integration
- Add analytics tracking
- Convert Tailwind CDN to production build
- Add loading states and skeleton screens
- Implement image lazy loading
- Add favorites/wishlist functionality
