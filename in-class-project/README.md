# MA COM Landing Page - Refactoring Project

**Course:** Web Communication (2026-27) – University of Milan  
**Assignment:** In-class exercise / Landing page refactor  
**Student:** Diana

---

## Overview

This project is a redesign and refactoring of the landing page for the Master's degree in Public and Corporate Communication (MA COM) at the University of Milan (<https://com.cdl.unimi.it/en>). 

Starting from the sample HTML discussed during lectures (`com_landing_seen_in_class.html`), the objective was to improve the page structure, accessibility, and visual hierarchy using semantic HTML5 and CSS Flexbox.

## Key Changes & Implementation

1. **Semantic HTML5 Structure**
   - Replaced generic container divs with semantic elements: `<header>`, `<nav>`, `<main>`, `<section>`, `<figure>`, and `<footer>`.
   - Used a description list (`<dl>`) in the study programme section to clearly distinguish between the three curriculum areas (Corporate, Public, and Research).

2. **Flexbox Layouts**
   - **Header:** space-between alignment for logo and navigation menu.
   - **Hero Section:** two-column split layout with headline and call-to-action on the left (using the Unimi brand red `#a6192e`) and the Torre Velasca photo on the right.
   - **Content Sections:** created reusable `.two-columns` flex containers for the about, video, and map sections.
   - **Quick Links:** three-column flex grid categorised by degree stages (before, during, and after).

3. **Styling & Assets**
   - **Typography:** paired *Merriweather* (serif, for headings) with *Source Sans 3* (sans-serif, for body text) loaded from Google Fonts.
   - **Grayscale Photo:** applied `filter: grayscale(100%)` to the computer lab photo to create a cleaner look and remove the blue screen reflection from the lab monitors.
   - **Embeds:** added the official YouTube presentation video using `youtube-nocookie.com` with a responsive 16:9 aspect ratio, and embedded an interactive Google Map for Via Conservatorio 7.

4. **Mobile Responsiveness**
   - Flex containers use wrapping (`flex-wrap: wrap`) with flexible basis sizes.
   - Added a `@media (max-width: 768px)` media query to stack navigation items and adjust typography and section padding on mobile screens.

## Project Structure

```
in-class-project/
├── index.html          # Page markup
├── styles/
│   └── style.css       # Stylesheet
├── imgs/               # Project images
│   ├── torrevelasca.jpg
│   └── sc_pol-10-cropped.jpg
└── README.md           # Project documentation
```

## How to View

Open `index.html` in any modern web browser (tested on Firefox and Chrome). No build tools or servers required.

## Sources & Credits

- Images: provided in course materials repository ([ale66/learn-web](https://github.com/ale66/learn-web))
- Course information, links, and video: official MA COM website ([com.cdl.unimi.it](https://com.cdl.unimi.it/en))
- Fonts: Google Fonts (*Merriweather*, *Source Sans 3*)
