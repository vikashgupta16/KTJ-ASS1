# KTJ-ASS1
A summer camp organized by Kshitij 2025 Summer Web Development &amp; AI Workshop.

# Media Discovery Platform

This repository contains a responsive, CSS-only media discovery website built with HTML and CSS. It showcases trending movies, popular shows, user reviews, and includes interactive components such as a hamburger menu, CSS-only modals, and watchlist toggles—all without JavaScript.

## Table of Contents
- [Demo](#demo)
- [Technologies & Resources](#technologies--resources)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
  - [1. Navbar](#1-navbar)
  - [2. Hero Section](#2-hero-section)
  - [3. Trending Movies](#3-trending-movies)
  - [4. Popular Shows](#4-popular-shows)
  - [5. User Reviews](#5-user-reviews)
  - [6. Footer](#6-footer)
  - [7. Responsive Design](#7-responsive-design)
- [Setup & Usage](#setup--usage)
- [License](#license)

## Demo
Open the `index.html` file in your browser to view the live site locally.
Else 

## Technologies & Resources
- **HTML5** for semantic structure.
- **CSS3** (Flexbox, Grid, animations, transitions).
- **Font Awesome** for icons (watchlist, social media, close, top button).
- **Google Fonts** (Poppins) for typography.
- CSS-only techniques:
  - Hamburger menu using a hidden checkbox toggle + `:checked` selector.
  - Modal dialogs for "Learn More" in Popular Shows via checkbox toggles.
  - Watchlist toggle (+ to ✓) using checkboxes and icon layering.
  - Smooth scrolling via `html { scroll-behavior: smooth; }`.

## Project Structure
```
ASS-1/
├── index.html        # Main HTML markup
├── style.css         # All site styles, animations, and responsive rules
└── Assets/           # Image assets & favicon
    ├── img1.jpg
    ├── img2.jpg
    ├── ...
    ├── Dp.jpg       # Default avatar for reviews
    └── icons8-netflix-256.png # Favicon
```

## How It Works
### 1. Navbar
- A fixed top navigation bar with the logo on the left.
- Links anchor-scroll to each section (`#hero`, `#trending`, etc.).
- On mobile (≤768px) the links collapse into a hamburger menu controlled by a hidden checkbox and CSS selectors.

### 2. Hero Section
- Uses Flexbox to split content into left (title, subtitle, button) and right (animated SVG graphic).
- The SVG has simple CSS and SMIL animations for a floating effect.
- CTA button scrolls to the Trending Movies section.

### 3. Trending Movies
- A grid (`.card-list`) of movie cards.
- Each card displays an image, title, description, duration, and a "Watch Now" link.
- Watchlist toggle implemented via a hidden checkbox; toggles Font Awesome plus/check icons on click.
- Hover and focus states use CSS transitions for interactive feedback.

### 4. Popular Shows
- Similar card layout for TV series.
- Each card has a "Learn More" label that toggles a modal overlay using a checkbox.
- Modal contains a detailed description and a follow-up "Watch Now" button.

### 5. User Reviews
- Displays user feedback cards with avatar, name, and text.
- Includes a styled review submission form (non-functional).

### 6. Footer
- Contains social media icon links (Font Awesome) with hover effects.
- Links to Terms & Conditions and Privacy Policy open in new tabs.
- Back-to-top button uses inline JS for smooth scroll (can be pure CSS if desired).

### 7. Responsive Design
- Media queries adjust layout for tablets (≤1100px) and mobiles (≤768px, ≤480px).
- Flex direction, font sizes, card widths, and spacing adapt to screen size.

## Setup & Usage
1. **Clone** or download this repository.
2. Ensure `index.html` and `style.css` are in the same directory.
3. Open `index.html` in your favorite browser.

_No build tools or servers required — pure HTML/CSS._

## License
This project is open source and available under the MIT License.
