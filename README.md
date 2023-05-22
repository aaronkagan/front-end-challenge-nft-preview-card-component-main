# NFT preview card

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

<img src="./images/screenshot-1.png" alt="NFT Preview Card" width=400px>

### Links

- [Repo](https://github.com/aaronkagan/nft-preview-card)
- [Live Site](https://fem-nft-prev-card.netlify.app/)

## My process

### Built with

- HTML5
- CSS
- Flexbox
- CSS Grid

### What I learned

During this process my biggest takeaway that I learned was how to use an absolutely positioned overlay to add a filter hover effect for the hover state

<img src="./images/screenshot-hover.png" alt="Hover State" width=300px>

```html
<div class="cube-image-container">
  <div class="cube-image-overlay">
    <img class="white-eye" src="/images/icon-view.svg" alt="White Eye" />
  </div>
  <img
    class="clear-cube-image"
    src="/images/image-equilibrium.jpg"
    alt="Clear Cube"
  />
</div>
```

```css
.cube-image-container {
  position: relative;
  font-size: 0;
}

.cube-image-overlay {
  position: absolute;
  display: grid;
  place-items: center;
  background-color: hsla(178, 100%, 50%, 0.5);
  width: 100%;
  height: 100%;
  border-radius: 1rem;
  opacity: 0;
}

.cube-image-overlay:hover {
  opacity: 100;
  cursor: pointer;
}

.clear-cube-image {
  border-radius: 1rem;
  width: 100%;
  height: 100%;
}

.white-eye {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
}
```

## Author

- Website - [Aaron Kagan](https://www.linkedin.com/in/aaron-kagan/)
- Twitter - [@aaronkagandev](https://www.twitter.com/aaronkagandev)
