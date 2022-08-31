# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Stats preview card component solution](#frontend-mentor---stats-preview-card-component-solution)
  - [Table of contents](#table-of-contents)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
  - [Author](#author)

### Screenshot

![](./images/screenshot1.png)
![](./images/screenshot2.png)

### Links

- Solution URL: [GitHub](https://github.com/StalinAM/statsPreviewCard.git)
- Live Site URL: [StalinAM](https://stalinam.github.io/statsPreviewCard/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow
- Responsive web design

### What I learned

Rearranges containers and changes image when width changes by a certain value.

```html
<picture class="image-container">
    <source srcset="./images/image-header-desktop.jpg" media="(min-width:1440px)">
    <img src="./images/image-header-mobile.jpg" alt="">
</picture>
<div class="information-container">
</div>
```

```css
@media (min-width: 1440px) {
    main {
        max-width: 1110px;
        grid-template-columns: repeat(2, 1fr);
    }
    .image-container {
        border-radius: 0 8px 8px 0;
        order: 2;
    }
    .information-container {
        text-align: start;
        padding:0 71px;
        order: 1;
    }
}
```

Rearrange containers from column to row.

```css
.information-container ul {
    grid-template-columns: repeat(3, 1fr);
}
```

## Author

- GitHub - [StalinAM](https://github.com/StalinAM)
- Frontend Mentor - [@StalinAM](https://www.frontendmentor.io/profile/StalinAM)