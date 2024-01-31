# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./screenshot.png)

### Links

- [Solution URL](https://github.com/liviagomesa/introductory-section)
- [Live Site URL](https://liviagomesa.github.io/introductory-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

1. I've learned how to use Font Awesome to get icons and use them within my webpage.

2. I've read more about attribute selection with CSS and then I could identify an efficiently way of selecting some elements instead of creating classes (this was something I used to do). For example, instead of creating a class named illustration to select my image, I inserted the code above:

   ```css
   img[alt="Illustration"]
   ```

   It was important to remember how to select all the descendants of an element using the character space (" "). I had to apply this to change the color of my icons and its borders, which are children of an "a" element.
   Other requirement was that only if the element "a" was under the mouse pointer its children should be selected. It was a challenge for me, which I solved with this code:

   ```css
   a:hover * {
   }
   ```

3. I could reinforce the use of flexbox. My strategy is to create a parent div and use display: flex whenever I want my items to be positioned side-by-side. After this, I apply a gap and centralize my content horizontally (justify-content: center) and vertically (required only if I have distinct-height flex items - align-items: center).

4. It was a challenge to me to create a circle around my icons. To do that, I had to create a div.icon and apply the following style to it:

   ```css
   .icon {
     display: flex;
     justify-content: center;
     align-items: center;
     border: solid 1px white;
     border-radius: 50%;
     width: 30px;
     height: 30px;
   }
   ```

   Flexbox was essential to me in this process.

### Continued development

I'm not completely comfortable with the concepts and techniques below - but I think they're useful and I want to refine by focusing in future projects:

- defining page's layout (columns and rows)
- content overflow
- css selectors

### Useful resources

- [CSS Icons - w3schools](https://www.w3schools.com/css/css_icons.asp) - This article gives some options to insert icons within your webpage.
- [How to Create Circular Backgrounds for your Font Awesome Icons](https://markheath.net/post/font-awesome-circle-background) - This helped me figure out how to create a circular border for my icon.
- [Stacking Icons - Font Awesome](https://fontawesome.com/docs/web/style/stack) - This is an alternative option to create the circle around the icon, but it didn't suit my case since the thin circle icon is paid and I my Font Awesome account is free.

## Author

- Frontend Mentor - [@liviagomesa](https://www.frontendmentor.io/profile/liviagomesa)
- LinkedIn - [@liviagomesa](https://www.linkedin.com/in/liviagomesa/)
