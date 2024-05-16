# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

- The HTML structure follows a typical layout for a recipe page.
- Sections include header, main content, ingredients, instructions, nutrition, and attribution.
- Semantic HTML elements like `<header>`, `<main>`, `<section>`, `<ul>`, `<ol>` are used appropriately.

- CSS file (`style.css`) provides styles for various elements of the HTML page.
- Font import from Google Fonts is done using `@import` statements.
- Typography is consistent across the page, with defined font families, sizes, and colors.
- Media query was used to create a responsive design, adjusting the layout and styles for smaller screens(mobile      devices).
- Flexbox is utilized for layout, providing flexibility and responsiveness.


### Screenshot

[Desktop-view](assets\images\Screenshot 2024-05-16 at 11-02-47 Frontend Mentor Recipe page.png)
[Mobile-view](assets\images\Screenshot 2024-05-16 at 11-41-31 Frontend Mentor Recipe page.png)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties

### What I learned

In the process of making this webpage, there we're some challenges I faced along the way. Below, are the code snippets(HTML and CSS) of the sections I found interesting:

```html
This was used to create a vertical table without the separating border for columns

 <div class="container">
        <h2>Nutrition</h2>
        <p>The table below shows nutritional values per serving without the additional fillings.</p>
      <div class="nutrition">
          <div class="nutrient">Calories</div>
          <div class="weight">277cal</div>
      </div>
      
      <div class="nutrition">
          <div class="nutrient">Carbs</div>
          <div class="weight">0g</div>
      </div>

      <div class="nutrition">
          <div class="nutrient">Protein</div>
          <div class="weight">20g</div>
      </div>
      
      <div class="nutrition">
          <div class="nutrient">Fat</div>
          <div class="weight">22g</div>
      </div>
    </div>
- Here is the CSS style for this section of HTML

      .nutrition{
          display: flex;
          border-bottom: 1px solid hsl(30, 18%, 87%);
          padding: 10px 0;
      }

      .weight{
          
          justify-self: center;
          font-weight: bold;
          color: hsl(14, 45%, 36%);
      }

      .nutrient, .weight {
          flex: 50%;
          font-family: "Outfit", sans-serif;
      }

      .container {
          margin-bottom: 25px;
      }

- Explanation:
      .nutrition: Elements with this class are displayed as flex containers, allowing for flexible layout. They have a bottom border for visual separation and padding for spacing.

      .weight: Elements with this class have their text centered horizontally, and the text fonts are styled as shown in the code snippet above.

      .nutrient, .weight: Both classes set their flex grow factor to 50%, allowing them to share equal space within their flex container.

      .container: Elements with this class have a margin at the bottom of 25 pixels, providing spacing between different sections of the page.
```

```css
This part of the code was used to make the website responsive enough for mobile devices with smaller screens.
Adjusting the font sizes, margins and padding according to the screen size(375px).

  @media (max-width: 375px) {
    body{
        width: 100%;
        background-color: white;
        padding: 0;
        margin: 0;
        border-radius:unset;
    }

    .header_image {
        width: 100%;
        border-radius: unset;
    }

    .header_image img {
        border-radius: inherit;
    }

    main, section, .container {
        margin-left: 20px;
        margin-right: 20px;
    }

    h1{
        font-size: 32px;
    }

    h2 {
        font-size: 24px;
    }

    .prep_list li::before, 
    .ing_list li::before, 
    .instruct_list li::before {
    margin-right: 3px;
    }
  }

```

### Continued development

- Responsive Designs - Ever since I started web development, i've always found this part cumbersome and I still haven't fully understood how to implement it. I plan to continue my learning process on this specific aspect of web development.

### Useful resources

- (https://www.W3schools.com) - This helped me understand the concept of ::before, ::after and ::marker attributes and also enlightened me in the use of flex in CSS. I really liked the way it was explained and will use it going forward.

## Author

- Website - [David Oladapo](https://www.your-site.com)
- Frontend Mentor - [@David-Oladapo](https://www.frontendmentor.io/profile/@David-Oladapo)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments
- W3 schools
- Xavier:)
