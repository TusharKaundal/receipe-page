# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

#### Desktop

![](/assets/screenshot/desktop.png)

#### Mobile

![](/assets/screenshot/mobile.png)

### Links

- Solution URL: [Github](https://github.com/TusharKaundal/receipe-page)
- Live Site URL: [Netlify](https://recipe-main-page-tush-bold.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

While going through development for this page came across nutrition article where table is to be formed so learned CSS property
nth-child() and nth-last-child().Which helped me target/select the column/rows and did styling so looks good.

Below are the code snippets used to provide style to nutrition article :

```html
<table class="nutrition-table">
  <tr>
    <td class="text-preset-4">Calories</td>
    <td class="text-preset-4-bold-cl">277kcal</td>
  </tr>
  <tr>
    <td class="text-preset-4">Carbs</td>
    <td class="text-preset-4-bold-cl">0g</td>
  </tr>
  <tr>
    <td class="text-preset-4">Protein</td>
    <td class="text-preset-4-bold-cl">20g</td>
  </tr>
  <tr>
    <td class="text-preset-4">Fat</td>
    <td class="text-preset-4-bold-cl">22g</td>
  </tr>
</table>
```

```css
.nutrition-table {
  padding: 0px 32px;
  border-collapse: collapse;
}

tr:nth-child(-n + 3) td {
  border-bottom: 2px solid var(--stone-150);
  padding-bottom: 12px;
}

tr:nth-last-child(-n + 3) td {
  padding-top: 12px;
}

tr td:nth-child(1) {
  padding-left: 32px;
}

tr td:nth-child(2) {
  padding-right: 32px;
}
```

### Useful resources

- [CSS Pseudo Classes](https://www.w3schools.com/css/css_pseudo_classes.asp) - This helped me in learning about CSS Pseudo Classes( nth-child() and nth-last-child() ).
- [Table Styling ](https://www.w3schools.com/css/css_table.asp) - This helped in better styling of tables how to provide border, padding.

## Author

- Website - [Tushar Kaundal](https://recipe-main-page-tush-bold.netlify.app/)
- Frontend Mentor - [@tusharkaundal](https://www.frontendmentor.io/profile/TusharKaundal)
