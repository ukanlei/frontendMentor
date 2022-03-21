# Frontend Mentor - QR code component solution

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learn](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

_A Shout-out to all the feedbacks helping me perfect my solution 🎉_

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

For this challenge, the width of the container containing the qr box is less than that of most mobile device, so I decided to not use media query as an experiment. [Read about result.](#no-media-what-will-happen)

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

### What I learned

To fix problem with flex item overflowing past the top edge and getting cut off with no accessible way to scroll up to see the rest of the content, I removed `align-item:center` and `justify-content:center` from `body`:

```css
body {
  align-items: center;
  justify-content: center;
}
```

and replaced it with `margin:auto` instead. The `auto` margins will assume the leftover space, centering item where there's leftover space, and switching to normal alignment when there's not.

```css
.container {
  margin: auto;
}
```

This was also my first experience using Figma. A fun learning process into the design tool and how to translate it into a live product.

### No @media? What will happen?

As mentioned in the overview, I decided not to use @media to see what would happen. What result did I get? Well, it depends.

For my first attempt, I gave my img a max-width of 18rem, same as my .box. The dimension of the box stays looking the same no matter the width of the screen. However, when the screen is at or under 320px, the box overflows, forcing users the need to scroll to see the rest of the content.

In my second attempt, I made the width of the img 100%. While this approach no longer results in an overflowing effect, the dimension of the box changes to fit within the screen.

### Useful resources

- [Semi-transparent box shadow](https://css-tricks.com/almanac/properties/b/box-shadow/) - Found this article helpful in visualizing possible options and create some cool effect with the box-shawdow property
- [Scroll limitation with overflowing flex](https://stackoverflow.com/questions/33454533/cant-scroll-to-top-of-flex-item-that-is-overflowing-container) - Super helpful in helping me figure out the issues I was having when using flex to center items.
- [Px vs. Rem](https://medium.com/user-experience-design-1/why-designers-should-move-from-px-to-rem-and-how-to-do-that-in-figma-c0ea23e07a15) - An article that helped me understand the difference between px vs rem and why one might choose one over the other when it comes to accessiblity.

## Author

- [Linkedin](https://www.linkedin.com/in/ukanlei/)
- Frontend Mentor - [@ukanlei](https://www.frontendmentor.io/profile/ukanlei)
