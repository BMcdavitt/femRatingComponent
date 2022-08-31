# Frontend Mentor - Interactive rating component solution

This is a solution to the [Interactive rating component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-rating-component-koxpeBUmI). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)

  - [What I learned](#what-i-learned)

  - [Useful resources](#useful-resources)




## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Select and submit a number rating
- See the "Thank you" card state after submitting a rating

### Screenshot

![](./images/Screenshot.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)


### What I learned

I struggled the most, honestly, with creating styled radio buttons.  This is the code that I landed on.

```html
      <div class="scoreInput">
        <input class="scoreInput" type="radio" name="score" id="1" value="1">
        <label class="scoreInputLabel" for="1">1</label>
        <input class="scoreInput" type="radio" name="score" id="2" value="2">
        <label class="scoreInputLabel" for="2">2</label>
        <input class="scoreInput" type="radio" name="score" id="3" value="3">
        <label class="scoreInputLabel" for="3">3</label>
        <input class="scoreInput" type="radio" name="score" id="4" value="4">
        <label class="scoreInputLabel" for="4">4</label>
        <input class="scoreInput" type="radio" name="score" id="5" value="5">
        <label class="scoreInputLabel" for="5">5</label>
      </div>
```
```css

.scoreInput {
  display: flex;
  justify-content: space-around;
}

.scoreInput input[type='radio'] {
  opacity: 0;
  position: fixed;
  width: 0;
}

.scoreInput label {
  background-color: #243b52;
  padding: 0.7rem;
  border-radius: 50%;
  width: 1.25rem;
  height: 1.25rem;
  text-align: center;
  margin-bottom: 2rem;
}

.scoreInput label:hover {
  background-color: hsl(25, 97%, 53%);
}

.scoreInput input[type='radio']:checked + label {
  background-color: hsl(217, 12%, 63%);
}

```




### Useful resources

- [How to style radio buttons](https://www.markheath.net/post/customize-radio-button-css) - This helped me understand how to style radio buttons.
