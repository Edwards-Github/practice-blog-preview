# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge] centering image (need to remember margin: auto works on block type elements and image is inline element)
  - [Screenshot](#screenshot)
  - [Solution] Solution: change image to a block size element with display: block; and margin: auto;

  - [The challenge] centering container to middle of the browser.
  - [Screenshot](#screenshot)
  - [Solution] Fixed this by making the body the full height of the "viewport height". Added "height: 100vh" to the body.
  - [Explanation] The issue is that the body is only as tall as its content right now — so there's no extra vertical space to center within.
	    	Think of it like this: if you wanted to center a book on a shelf, the shelf needs to actually be taller than the book. 
	    	Right now your "shelf" (the body) is the same height as the "book" (the card).

  - [The challenge] On mobile view the whole thing is zoomed in so you can only see portions of the whole thing.
  - [Screenshot](#screenshot)
  - [Solution] I had property max-width: 375px; on the container class, but the phone screen is exactly 375px wide so it left no space left and right of container.
  - [Explanation] Key insight: width: 100% means 100% of the parent's width. And the parent is the body. So if the body had some padding on the sides, the container's
	   	100% would naturally be smaller than the screen (this was the fix)!

  - [The challenge] Course image was overflowing when switched to mobile
  - [Screenshot](#screenshot)
  - [Solution] fixed by adding width: 100%.
  - [Explanation] If you don't set a width on image then it defaults to natural size (whatever size the image file is).

- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned]
	a. margin: auto only works on block elements, so you changed the image to display: block
	b. align-items: center needs the parent to have height, so you used height: 100vh
	c. width: 100% on a child respects the parent's padding, so adding padding to body gave the card breathing room on mobile.
  - [Useful resources] www.frontendmentor.io
  - [AI Collaboration]Claude
- [Author](#author)
- [Acknowledgments](#acknowledgments)www.frontendmentor.io

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

<img width="2547" height="1362" alt="image" src="https://github.com/user-attachments/assets/92896af4-e2df-4a85-b126-192365c0e57b" />

### Links

- Solution URL: https://github.com/Edwards-Github/practice-blog-preview
- Live Site URL: https://edwards-github.github.io/practice-blog-preview/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned
	1. margin: auto only works on block elements, so you changed the image to display: block
	2. align-items: center needs the parent to have height, so you used height: 100vh
	3. width: 100% on a child respects the parent's padding, so adding padding to body gave the card breathing room on mobile


### Continued development

	1. Want to continue working on centering images and containers.
	2. Want to continue getting better at making websites mobile friendly as well.
	3. Want to continue getting better at height and width and understanding the nuances.

### AI Collaboration

Describe how you used AI tools (if any) during this project. This helps demonstrate your ability to work effectively with AI assistants.

- What tools did you use (e.g., ChatGPT, Claude, GitHub Copilot)? Claude
- How did you use them (e.g., debugging, generating boilerplate, brainstorming solutions)? I used Claude as a patient mentor walking me through what is going on. It challenges my understanding as opposed to giving me the answer.

## Author

- Website - [Edward] (https://github.com/Edwards-Github)
- Frontend Mentor - [@Edwards-Github] (https://www.frontendmentor.io/profile/Edwards-Github)
