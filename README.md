# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./images/screenshot.png)

### Links

- Solution URL: [https://github.com/Danedey/practice-four-cards](https://github.com/Danedey/practice-four-cards)
- Live Site URL: [https://danedey.github.io/practice-four-cards/](https://danedey.github.io/practice-four-cards/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

when you have different sections that later are going to be displayed as cards in your website, you can wrap them all inside a unordered list like:

from this:
```html

<section>
  <h2>Supervisor</h2>
  <p>Monitors activity to identify project roadblocks</p>
</section>

<section>
  <h2>Team Builder</h2>
  <p>Scans our talent network to create the optimal team for your project</p>
</section>

<section>
  <h2>Karma</h2>
  <p>Regularly evaluates our talent to ensure quality</p>
</section>

<section>
  <h2>Calculator</h2>
  <p>Uses data from past projects to provide better delivery estimates</p>
</section>
          
```

to this
```html

<ul>
  <li> 
    <section>
      <h2>Supervisor</h2>
      <p>Monitors activity to identify project roadblocks</p>
    </section>
  </li>
  <div class="column-container"> 
    <li >
      <section>
        <h2>Team Builder</h2>
        <p>Scans our talent network to create the optimal team for your project</p>
      </section>
    </li>
    <li >
      <section>
        <h2>Karma</h2>
        <p>Regularly evaluates our talent to ensure quality</p>
      </section>
    </li>
  </div>
  <li >
    <section>
      <h2>Calculator</h2>
      <p>Uses data from past projects to provide better delivery estimates</p>
    </section>
  </li>
</ul>

```

and another thing i realized is that when you change the css propertie from flex-direction: column to flex-direction: row, these two properties justify-content and align-items exchange behavior.



### Continued development

i want to sharp my layout making because i didnt feel confortable enough with that aproach i used to make a diamon like figure with 4 cards. i needed to put two card in a column just in the center and a card beside each left and right. so i wrapped these two card in a div container and then center it.

### Useful resources

- [CSS_layout Flexbox](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Flexbox) - this help me to understand why my flex container centers in the x axis using justifly-content: center when you set a flex-direction to column. it has something to do with the main axis.
- [CSS_layout/Grids](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Grids) - this article helped me to understand how to use grid areas for a custom layout.

### AI Collaboration

i used copilot to ask how can i handle font-sizes in my page so that i ended up using good practices, it was ok.

i used claude again to compare my aproach at structuring html files, i learnt a few things.

## Author

- Frontend Mentor - [@Danedey](https://www.frontendmentor.io/profile/Danedey)
