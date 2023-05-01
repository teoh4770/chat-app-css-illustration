# Frontend Mentor - Chat app CSS illustration
## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

- Mobile View

![Screen Shot 2023-05-01 at 14 34 08](https://user-images.githubusercontent.com/98545971/235507562-6661bf02-c93e-45a8-ac49-ac54a6cf273d.png)

- Desktop view

![Screen Shot 2023-05-01 at 14 34 42](https://user-images.githubusercontent.com/98545971/235507670-ea77b543-96e3-4517-b3fb-4cf659bd2aad.png)

### Links

- Solution URL: [https://github.com/teoh4770/chat-app-css-illustration](https://github.com/teoh4770/chat-app-css-illustration)
- Live Site URL: [https://teoh4770.github.io/chat-app-css-illustration/](https://teoh4770.github.io/chat-app-css-illustration/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- BEM naming convention
- Custom UI Background and animation

### What I learned

To see how you can add code snippets, 
see below:

html
```
<div class="blob blob--primary rotate"></div>
<div class="blob blob--secondary rotate"></div>
```

css
```
/* 1. creating a blob shape div with border-radius */
.blob {
  --blob-width: 432px;
  --half: calc(var(--blob-width) * -0.2);
  position: absolute;
  width: var(--blob-width);
  aspect-ratio: 1;
  border-radius: 43% 57% 29% 71% / 35% 71% 29% 65%;
  background: linear-gradient(var(--light-magenta), var(--light-violet));
}

/* 2. using sibling selector to apply styling  */
.phone-chat__bubble--primary + .align-right,
.align-right + .phone-chat__bubble--primary {
  margin-top: 12px;
}

/* 3. implement the rotation animation to blob */
@keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}
```

### Useful resources

- [Creating blob shape with border-radius](https://9elements.github.io/fancy-border-radius/)
- [Google icons](https://fonts.google.com/icons)

## Author

- Website - [CheeKianTeoh](https://github.com/teoh4770/)
- Frontend Mentor - [teoh4770](https://www.frontendmentor.io/profile/teoh4770)

