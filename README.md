# Frontend Mentor — QR Code Component

This is my solution to the [QR Code Component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). I built it while practicing semantic HTML, CSS layout, and responsive design.

## Table of contents

- [Overview](#overview)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Recreate the provided QR code card design for desktop and mobile using HTML and CSS. The card shows a QR code, a heading, and a short description inviting visitors to explore Frontend Mentor.

### Links

- **Repository:** [View source on GitHub](https://github.com/Jeremiah-Akpor/frontendmentor-qr-code-component)
- **Live site:** [View QR Code Component on GitHub Pages](https://jeremiah-akpor.github.io/frontendmentor-qr-code-component/)
- **Frontend Mentor solution:** Not submitted yet.

_A screenshot of the finished implementation can be added here after deployment._

## My process

### Built with

- Semantic HTML5
- CSS (separate stylesheet)
- Flexbox for centering and arranging content
- CSS box model and `box-sizing: border-box`
- Responsive image sizing (`width: 100%`)
- Media queries and logical properties (`padding-inline`)
- Google Fonts — Outfit

No JavaScript, CSS framework, React, or Next.js was used.

### What I learned

This challenge helped me understand the difference between **changing an element's size** and **adding space around it**.

- **Parent vs. child responsibilities:** `main` controls the card's position; `.card` controls padding around its contents; the paragraph's `max-width` controls text wrapping.
- **Flexbox centering:** With the default row direction, `justify-content` aligns along the horizontal main axis and `align-items` along the vertical cross axis. The parent needs enough height for vertical centering to be noticeable.
- **Box sizing:** With `border-box`, padding is included in a declared width, while margins remain outside it.
- **Responsive spacing:** Instead of shrinking the card just to create distance from mobile viewport edges, I used `padding-inline` on its parent.
- **Typography:** Changing `max-width` affects where text wraps, whereas `line-height` changes the space between text lines.

An example of a responsive layout technique I practiced:

```css
@media (max-width: 600px) {
  main {
    padding-inline: 15px;
  }
}
```

I first built the semantic HTML structure, then refined the CSS by comparing the browser output with the supplied desktop and mobile images.

### Continued development

I want to keep practicing:

- Estimating spacing and proportions from static reference images when exact measurements aren't provided.
- Choosing between parent padding, child dimensions, and margins based on the layout problem.
- Testing designs at multiple viewport widths, including narrow mobile screens.
- Improving semantic HTML, accessibility, and visual consistency.

### Useful resources

- [MDN — CSS box model](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Box_model)
- [MDN — Flexbox basics](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
- [MDN — padding-inline](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-inline)
- [Frontend Mentor style guide](./style-guide.md) — colors, font, and design reference widths for this challenge.

### AI collaboration

I used ChatGPT as a **learning companion and code reviewer**, rather than asking it to generate the finished page. I wrote and adjusted the HTML and CSS myself. The assistant reviewed my workspace, pointed out potential layout issues, explained concepts such as the box model and Flexbox axes, and guided me through small experiments. That helped me understand *why* changes worked instead of just copying a solution.

## Author

- GitHub — [Jeremiah-Akpor](https://github.com/Jeremiah-Akpor)
- Challenge — [Frontend Mentor QR Code Component](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H)
