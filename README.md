# Frontend Mentor - Interactive pricing component solution

This is a solution to the [Interactive pricing component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-pricing-component-t0m8PIyY8). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Use the slider and toggle to see prices for different page view numbers

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow
- Svelte Framework

### What I learned

I felt like using Svelete was a bit overkill for this project, but I found it extremely easy and straightforward to use. It helped where I needed to use Javascript. Making each piece of the website its own component certainly helped as well ensuring that each piece is stylized appropiately. 

I wanted to talk a bit about how neat Svelte is. I was easily able to change the website based off the screen width. Check this out:

```
{#if window.innerWidth >= 1440}
  <p id="discount-special">-25% discount</p>
{:else}
  <p id="discount-special">-25%</p>
{/if}
```

Same with the slider, I'm referencing a Javascript variable in my HTML. A big game changer if you ask me.

```
<script>
  let range = 16;

  function handleSlide() {
      range = this.value;
  }
</script>

<div class="price">
  <p id="big-money">${range.toString() + '.00'}</p>
  <p id="month">/ month</p>
</div>
```

### Continued development

In future projects, I hope to continue using Svelte. I hope to do something a bit more ambitious with Javascript.

### Useful resources

- [Customizing the input thumb](https://css-tricks.com/styling-cross-browser-compatible-range-inputs-css/) - I looked through so many examples and none were helping me until I found this resource. I'm not sure what made the gears start spinning but extracting bits here helped me get a better idea of what was happening.
- [Creating the toggle switch](https://danklammer.com/articles/simple-css-toggle-switch/) - Shoutout to Dan Klammer creating this straight forward toggle switch.
- [Using flex](flexboxfroggy.com) - I started using `display: flex` more in this project and I've finished the project faster by practicing on here.

## Author

- GitHub - [Brandon Nhem](https://www.github.com/brandonnhem)
- Frontend Mentor - [@brandonnhem](https://www.frontendmentor.io/profile/brandonnhem)

## Acknowledgments

Special thanks to ApplePieGiraffe on the Frontend Mentor Slack for providing guidance. For anyone out there worried about getting it right, here's some knowledge for you: 

**"Don't worry too much about your solution not matching up with the original design in the design preview perfectly—that isn't the main point of Frontend Mentor challenges and it's often a little more difficult and time-consuming than is worth it to get very accurate results."**

This has definitely helped me from pixel peeping to make sure it's just right.
