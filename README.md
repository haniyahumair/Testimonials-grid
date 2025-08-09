# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge
Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See a responsive testimonials grid that adapts from desktop to mobile


### Screenshot

<img width="1261" height="675" alt="image" src="https://github.com/user-attachments/assets/3c918912-c011-4b05-a415-68d61c5da573" />

<img width="488" height="561" alt="image" src="https://github.com/user-attachments/assets/6757515d-b69e-427d-9bf9-acf46c97cd5d" />

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (CSS variables)
- CSS Grid for desktop layout
- Flexbox for mobile layout
- Mobile-first workflow
- Google Fonts (Barlow Semi Condensed)

### What I learned

This project helped me understand the power of CSS Grid's `grid-template-areas` for creating complex layouts. I learned how to create a responsive design that switches from a grid layout on desktop to a simple column layout on mobile.


```css
.testimonials-cards {
  display: grid;
  grid-template-areas: 
    "daniel daniel jonathan kira"
    "jeanette patrick patrick kira";
}

#daniel-card { grid-area: daniel; }

```
```mobile query
@media (max-width: 768px) {
  .testimonials-cards {
    display: flex;
    flex-direction: column;
  }
}
```
I also learned how to properly layer elements using `z-index` and position the decorative quote icon behind the text content.

### Continued development

Areas I want to focus on in future projects:

- More advanced CSS Grid techniques and subgrid
- Better understanding of accessibility in grid layouts
- Exploring CSS animations for hover effects
- Learning more about responsive typography

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
