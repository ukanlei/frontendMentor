# Frontend Mentor - QR code component solution

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Issues & Solutions](#issues--solutions)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). In this solution:

- Users can view the optimal layout depending on their device's screen size.

### Screenshot

![](images/qr-screenshot.png)

### Links

- Solution URL: [Github](https://github.com/ukanlei/frontendMentor/tree/master/qr-code-component-main)
- Live Site URL: [Netlify](https://cocky-mestorf-38a51c.netlify.app)

## My Process

### Built with

- HTML5
- CSS3
- Flexbox
- Mobile-first workflow

### Issues & Solutions

To fix problem with overflowing flex item getting cut off with no accessible way to scroll to see more of the content, I removed `align-item:center` and `justify-content:center` from `body`:

```css
body {
  align-items: center;
  justify-content: center;
}
```

and replaced it with `margin:auto` instead:

```css
.container {
  margin: auto;
}
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

### Useful resources

- [Semi-transparent box shadow](https://css-tricks.com/almanac/properties/b/box-shadow/) - Found this article helpful in visualizing possible options and create some cool effect with the box-shawdow property
- [Scroll limitation with overflowing flex](https://stackoverflow.com/questions/33454533/cant-scroll-to-top-of-flex-item-that-is-overflowing-container) - Super helpful in figuring out overflowing flex item issue and understanding issues that may arise when using flex to center items.

## Author

- [Linkedin](https://www.linkedin.com/in/ukanlei/)
- Frontend Mentor - [@ukanlei](https://www.frontendmentor.io/profile/ukanlei)
