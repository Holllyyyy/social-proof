# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

Social proof section built with CSS Grid. Use of media query and make it responsive for small devices.

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

First I write my HTML file, where I had to think and to be careful about position of each element on the page, because there are differences between mobile and deskop view. After it I go to write my CSS reset. I started to write CSS for mobile first. I used display Grid for mobile where is part for my three review what I named section-card. That looks like this:

```css
.card {
  padding: 2rem;
  display: grid;
  grid-template-columns: repeat(3, 2fr 2fr);
}
.card__img {
  grid-column: 1/2;
  grid-row: 2;
}
.card-heading {
  grid-column: 3/7;
  grid-row: 2;
}
.card-heading-one {
  font-weight: 700;
}
.card-p {
  margin-top: 1rem;
  grid-column: 1/-1;
  grid-row: 3;
}
```

So when I got how I wanted my cards to look like, I move on on the desktop view.
Interesting part and something what I learned is also about this cards. I was thinking how can I make cards , to be like in the design, how i can move one up and other down.. After some time, I got idea.

```css
.section-cards {
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}
.card-heading-one {
  font-weight: 700;
}
.card-heading-two,
.card-text {
  font-weight: 400;
  font-size: var(--fs-200);
}
.card + .card {
  margin-top: 0;
}
.card-one {
  align-self: start;
}
.card-two {
  align-self: center;
}
.card-three {
  align-self: end;
}
```

So here, I just used align-self what was very useful , and I finished it.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

With this challenge I practice more and learn more how to do positioning with CSS Grid.

### Continued development

I will continue next with challenge, from Frontend Mentor. I want to practice and improve my HTML and CSS skills.

## Author

- Website - [Svetlana Jokic](https://my-portfolio-hollyy.netlify.app/)
- Frontend Mentor - [@Holllyyyy](https://www.frontendmentor.io/profile/Holllyyyy)
- Twitter - [@svetlanajokic](https://twitter.com/svetlanajokic)
- LinkedIn - [@Svetlana Jokic](https://www.linkedin.com/in/svetlana-jokic-787432100/)
