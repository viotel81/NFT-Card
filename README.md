# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![images/screenshot.png]

### Links

- Solution URL: [https://github.com/viotel81/NFT-Card.git]
- Live Site URL: [https://viotel81.github.io/NFT-Card/]

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

My biggest takeaway from this exercise is the active state of the equilibrium image. I have scrolled through quite some online resources to come up with the below CSS solution.

```css
.card-header {
    height: 270px;
    position: relative;
}

.card-header img {
    width: 100%;
    height: 100%;
    border-radius: 10px;
    object-fit: cover;
}

.hover-view {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    background-color: rgba(0, 255, 247, 0.4);
    transition: 0.5s ease;
    opacity: 0;
    border-radius: 10px;
}

.card-header:hover .hover-view {
    opacity: 1;
    cursor: pointer;
}

.eye-image {
    width: 40px;
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}
```
### Continued development

I would still need some practice on the manipulation of the divs for hovering effects. They involve a lot of floating techniques which I am still not fully comfortable with, as I love using Flexbox for such matters:)

### Useful resources

- [https://www.w3schools.com/howto/howto_css_image_overlay.asp] - This helped me with the image hover effect.

## Author

- Website - [https://github.com/viotel81]
- Frontend Mentor - [https://www.frontendmentor.io/profile/viotel81]
