# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![QR code component](./screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I Learned

One of the biggest takeaways from this project was understanding how to make layouts more responsive using `clamp()` and proportional scaling.

I learned that `clamp(min, preferred, max)` allows you to define a value that grows fluidly with the viewport (using units like `vw`) but never goes below a set minimum or above a maximum. This is especially useful for paddings, margins, and font sizes.

To calculate proportional scaling, I used the formula:

mobile padding = desktop padding × (mobile width ÷ desktop width)

For example, a top padding of `230.5px` at `1440px` scales down to about `60px` at `375px`.

Here’s how I implemented it with `clamp()` to keep it fluid but bounded:

```css
  padding-top: clamp(60px, 16vw, 230.5px);
  padding-bottom: clamp(60px, 16vw, 230.5px);
  padding-left: clamp(146px, 39vw, 560px);
  padding-right: clamp(146px, 39vw, 560px);
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

## Author

- Frontend Mentor - [@Mell-o](https://www.frontendmentor.io/profile/Mell-o)
