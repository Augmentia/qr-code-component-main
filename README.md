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

## Overview

I started off with this QR card project to get a little more familiar with CSS. I didn't want to distract from that and stayed with HTML and CSS throughout the project.

### Screenshot

![Image Preview](./images/preview.PNG)

### Links

- Solution URL: [Add solution URL here](https://github.com/Augmentia/qr-code-component-main)
- Live Site URL: [Add live site URL here](https://augmentia.github.io/qr-code-component-main/)

## My process

I started with HTML and CSS. I took the information initially given such as colors and made variables for the colors. I implemented the colors, then the central container with CSS Grid. I took the image and put it in the container along with the text, and made it a fixed size so it didn't scale. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

So in the process of developing the QR card I had this strange bug where the content specified in the CSS "grid-area" wasn't going in it's respective area.
As most programming bugs are, it had to do with using quotations on the wrong thing. Here is an example:

```css
.example {
    display: grid;
    grid-template-columns: auto 200px auto ;
    grid-template-rows: 20vh 350px 20vh;
    grid-template-areas: 
    ". . ."
    ". content ."
    ". . .";
  }

  .incorrect {
    grid-area: "content";
  }

  .correct {
    grid-area: content;
  }
```

### Continued development

I really like the look of the component, and if I needed a QR component for a project I could see myself pulling something like this and making it dynamic for something like a mobile web app. A cursory view of npm show a package called "qrcode", which I'm sure I could plug in to make the QR whatever I wanted.

### Useful resources

- [CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - This website helped me get into CSS Grids.

## Author

- Frontend Mentor - [@Augmentia](https://www.frontendmentor.io/profile/Augmentia)

