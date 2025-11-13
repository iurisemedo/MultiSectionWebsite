# #1 FREE LEAKS - Model Showcase Website

## Overview
A high-conversion, single-page model showcase website built with Tailwind CSS, featuring a clean Apple-inspired design aesthetic with smooth animations and mobile-first responsive layout.

## Project Structure
```
.
├── index.html              # Complete single-file website (HTML, CSS, JS)
├── attached_assets/        # Model images and media files
└── replit.md              # This file
```

## Features

### Hero Section
- Large, bold "#1 FREE LEAKS" heading in accent color (#87CEEB)
- "Best prices on the market" subheading
- Two prominent CTA buttons: "Join Discord" and "Join Telegram"
- Smooth fade-in and slide-up animations on scroll

### Model Gallery
- **30 model cards** displayed in a responsive grid
  - 2 columns on mobile
  - 3 columns on tablet
  - 4 columns on desktop
- **Real-time search functionality** - filters models as you type
- Each card includes:
  - High-quality model image
  - Model name
  - Price in euros (€)
  - "Buy Now" action button
- Hover effects with elevation and shadow
- Scroll-triggered fade-in animations for each card

### Premium Upgrade Modal
- Accessible via navigation bar button
- Full-screen overlay modal with 3 pricing tiers:
  - **Weekly**: €6.99/week
  - **Monthly**: €19.99/month (highlighted as "POPULAR")
  - **Lifetime**: €59.99 (one-time payment)
- Features list:
  - Access to all models
  - Custom model requests
- Smooth animations when opening
- Close via X button, outside click, or Escape key

## Technical Implementation

### Design System
- **Background**: #FAFAFA (off-white)
- **Primary Text**: #000000 (black)
- **Accent Color**: #87CEEB (light blue)
- **Fonts**:
  - Headings: Poppins Bold
  - Body: Inter (400, 500, 600 weights)

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
