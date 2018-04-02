# SASS Cheatsheet

### What is SASS?

* Sass (Syntactically Awesome Style Sheets) is a CSS preprocessor. It is to CSS what CoffeeScript is to Javascript. Sass adds a feature set to your stylesheet markup that makes writing styles fun again.

### Features

Fully CSS-compatible
Language extensions such as variables, nesting, and mixins
Many useful functions for manipulating colors and other values
Advanced features like control directives for libraries
Well-formatted, customizable output

### How to install

* You need Ruby installed prior to use SASS
* Install SASS (on Mac)
  $sudo gem install sass
* Check the version of the sass
  $ sass --version

[more info about install](https://sass-lang.com/install)

### Sass vs Scss

Sass has more simple code like Ruby and Scss is more like CSS. But Scss is more popular and widely used.

### Variables: Sass brings variables to CSS.

EX)
$primaryColor: #eeccff;

body {
background: $primaryColor
}

$firstValue: 62.5%;

p {
font-size: $firstValue
}

$container-width: 100%;

.container {
width: $container-width;
}

### Functions

* One of the best part of Sass is that it's built in functions.
  EX)
  $color: hsl(120deg, 100%, 50%)

More examples are below.
http://sass-lang.com/documentation/Sass/Script/Functions.html

### Nesting

EX)
.container {
width: 100%;
h1 {
color: red;
}
}

### Imports

* It allows you to break your styles into separate files and import them into one another. This does wonders for organization and speed of editing.

EX)
@import "grids.scss";
@import "grids"; (don't even really need the extension)

### Extends & Placeholders

* @extend directive is an outstanding way to inherit already existing styles.
  EX)
  .input {
  border-radius: 3px;
  border: 4px solid #ddd;
  color: #555;
  font-size: 17px;
  padding: 10px 20px;
  display: inline-block;
  outline: 0;
  }

.error-input {
@extend .input;
border:4px solid #e74c3c;
}

### Mixins

* It allows you to include styles the same way @extend would, but with the ability to supply and interperet arguments.

### Youtube videos I've watched to learn

* SASS Tutorial by Derek Banas

https://www.youtube.com/watch?v=wz3kElLbEHE
-> This is the most viewed SASS video on Youtube but it was hard for the beginners like me.
I might come back later after learning more.

* Sass & SCSS Tutorial for Beginners by thenewboston

https://www.youtube.com/watch?v=sCbXTrsl7NU
https://www.youtube.com/watch?v=3hC2cbjvIXc
https://www.youtube.com/watch?v=t9IHDRWx1dQ&list=PL6gx4Cwl9DGBxQO2r_kmxn-0UqL_Rkj0t&index=3

### Good tutorials to learn

* Getting Started with SASS (with Interactive Examples)
  https://scotch.io/tutorials/getting-started-with-sass

- The Sass Way
  http://www.thesassway.com/
- Sass News
  https://twitter.com/SassNews

### Some Sass(Scss) Practice I made on Codepen

https://codepen.io/hyojinsarchet/pen/rdKjmL
