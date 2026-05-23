# Roberto Web - Project Documentation

## Project Overview

> **Note:** This project was developed as part of the **Saylani Mass IT Training's Coding Night 2025 (Hackathon) - Coding and Creativity Night**.

**Roberto** is a static single-page website template for a luxury hotel/resort. It showcases hotel amenities, room bookings, testimonials, and contact information with a modern, responsive design.

### Deployment

- [GitHub URL](https://github.com/sheikh-mohammad/frontend-ui-projects/tree/main/roberto-web)
- [Live URL](https://roberto-web.netlify.app/)

### Key Features

- **Hero Section**: Full-screen carousel with booking form overlay
- **About Section**: Hotel introduction with image grid layout
- **Services**: Icons displaying amenities (transportation, spa, restaurant, bar)
- **Room Showcase**: Carousel displaying room types with pricing and features
- **Testimonials**: Guest reviews section
- **Blog/News**: Latest news and events cards
- **Contact CTA**: Call-to-action banner
- **Footer**: Newsletter subscription, links, and social media

### Technology Stack

| Category       | Technology                                         |
| -------------- | -------------------------------------------------- |
| **HTML**       | HTML5 semantic structure                           |
| **CSS**        | Custom CSS + Bootstrap 5.3.8                       |
| **Icons**      | Font Awesome 7.0.1                                 |
| **Fonts**      | Poppins (local TTF)                                |
| **JavaScript** | Bootstrap Bundle (for carousel, dropdowns, modals) |

### Color Scheme

```css
--primary: #1cc3b2 /* Teal accent color */ --secondary: #2a303b
  /* Dark navy for headers/top bar */;
```

## Project Structure

```
roberto-web/
├── index.html          # Main HTML file (547 lines)
├── style.css           # Custom styles (399 lines)
├── README.md             # Project documentation
└── assets/
    ├── fonts/
    │   └── Poppins-Regular.ttf
    └── images/
        ├── about/      # About section images
        ├── blog/       # Blog post thumbnails
        ├── companies/  # Partner/company logos
        ├── contact/    # Contact section background
        ├── footer/     # Footer logo
        ├── hero/       # Hero carousel images (3)
        ├── logo/       # Site logo
        ├── plans/      # Room plan images
        ├── project/    # Project gallery images
        ├── service/    # Service icons (5)
        └── testinomial/ # Testimonial background
```

## Building and Running

### Quick Start

Since this is a static website, simply open `index.html` in a browser:

```bash
# Option 1: Direct file open
start index.html

# Option 2: Use a local server (recommended for proper asset loading)
npx serve .
# or
python -m http.server 8000
# or
php -S localhost:8000
```

### Development Server

No build process required. Edit files directly and refresh the browser.

## Development Conventions

### CSS Patterns

- **CSS Variables**: Use `--primary` and `--secondary` for consistent theming
- **Transitions**: Standard 500ms transitions for hover effects
- **Utility Classes**: Heavy use of Bootstrap utilities (`py-`, `px-`, `d-flex`, `gap-`, etc.)
- **Custom Classes**: Section-specific classes (`.hero-section`, `.booking-section`, `.testimonial-section`)

### HTML Patterns

- **Bootstrap Grid**: Uses Bootstrap's grid system (`row`, `col-*`, `container`, `container-fluid`)
- **Semantic Sections**: Content organized in `<section>` tags
- **Flexbox**: Extensive use of flex utilities for layout

### Image Assets

- All images are PNG format
- Stored in categorized subdirectories under `assets/images/`
- Naming convention: `{section}/{section-name}-{number}.png`

## Key Components

### Navigation

- Fixed top bar with contact info and social icons
- Main navbar with dropdown menu
- "Book Now" CTA button

### Booking Form

- Floating form overlapping hero section
- Fields: Check-in, Check-out, Rooms, Adults, Children
- "Check Availability" submit button

### Room Carousel

- Split layout: image (50%) + details (50%)
- Dark background for details panel
- Price highlighting in accent color

### Interactive Elements

- Hover effects on cards (translateY animation)
- Dropdown menus on hover
- Image zoom on hover (about section)
- Project slide reveal on hover

## Known Considerations

1. **Font Awesome Version**: Uses v7.0.1 from CDN - ensure internet connectivity for icons
2. **Bootstrap Version**: References 5.3.8 from CDN
3. **Local Font**: Poppins font loaded from local `assets/fonts/` directory
4. **Responsive Design**: Bootstrap handles responsiveness; custom CSS adds refinements
5. **No JavaScript Logic**: All interactivity via Bootstrap components only

## Usage

This template is intended for:

- Hotel/resort websites
- Hospitality business landing pages
- Learning Bootstrap 5 layout patterns
- Quick prototyping of accommodation booking interfaces

**Attribution**: Template by [Colorlib](https://colorlib.com)
