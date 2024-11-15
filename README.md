# Frontend Mentor - Testimonials Grid Section Solution

![Design preview for the Testimonials Grid Section coding challenge](./design/desktop-preview.jpg)

## Welcome! 👋

Thank you for checking out this front-end coding challenge.

This is a solution to the [Testimonials Grid Section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7 ). These challenges help you build real-world projects and enhance your front-end development skills.

## Table of Contents

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screens](#screens)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Code Snippet](#code-snippet)
  - [Useful Resources](#useful-resources)

## Overview

### The Challenge

Your users should be able to:

- View the optimal layout for the testimonials grid depending on their device's screen size.
- See hover states for all interactive elements on the page.
- Experience a responsive design with a clean, professional look.

### Screens

#### Desktop Preview
  <img src="./assets/images/desktop-preview.png" alt="Desktop Preview" />

#### Tablet Preview
  <img src="./assets/images/tablet-preview.png" alt="Tablet Preview" />

#### Mobile Preview
  <img src="./assets/images/mobile-preview.png" alt="Mobile Preview" />

### Links

- Solution URL: [GitHub Repository](https://github.com/harisdev-netizen/testimonials-grid-section)
- Live Site URL: [Live Demo](https://testimonials-grid-sec.netlify.app/)

## My Process

### Built With

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid for layout
- Mobile-first workflow
- Responsive design techniques
- [Google Fonts](https://fonts.google.com/) - For custom typography

### What I Learned

This project enhanced my understanding of:

- Creating responsive grid layouts using `grid-template-areas`.
- Utilizing CSS custom properties for theme-based design.
- Building hover effects with transitions for an interactive user experience.
- Applying media queries for seamless design on different screen sizes.

### Code Snippet

Below is an example of the CSS Grid layout used in this project:

```css
.grid-container {
  display: grid;
  grid-template-areas:
    "card1 card1"
    "card2 card3"
    "card4 card5";
  grid-gap: 1.5rem;
  margin: 0 auto;
  max-width: 1200px;
}

@media (min-width: 768px) {
  .grid-container {
    grid-template-areas:
      "card1 card1 card2 card2"
      "card3 card3 card4 card5";
  }
}

.card1 {
  grid-area: card1;
  background-color: var(--primary-color);
  padding: 2rem;
  border-radius: 10px;
  color: #fff;
}
