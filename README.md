# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![](./images/screenshot.jpg)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/landing-page-first-time-using-sass-ryNhnommc](https://www.frontendmentor.io/solutions/landing-page-first-time-using-sass-ryNhnommc)
- Live Site URL: [https://kpax10.github.io/profile-card-component-main/](https://kpax10.github.io/profile-card-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- Sass
- Sass variables, functions
- Flexbox

### What I learned

-I learned that sass functions exist and can be used to create dry code.  The below function creates a flex display, allowing me to input the flex direction as an argument.
```css
@mixin flex-center($direction) {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: $direction;
}
```

-The background images were moving left and right on the page giving me issues.  I realized the 'background-position' property needed to be using 'vw' and 'vh' instead of px or %.
```css
body {
    height: 100vh;
    background-image: url(../images/bg-pattern-top.svg), url(../images/bg-pattern-bottom.svg);
    background-repeat: no-repeat, no-repeat;
    background-position: right 50vw bottom 38vh, left 48vw top 51vh;
}
```
-Github pages require background images to have a '../' in front of the link to be functional.
```css
.container-top {
    background-image: url(../images/bg-pattern-card.svg);
}
```