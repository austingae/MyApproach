# SASS

To use SASS, you must have installed two extensions: Sass and Live Sass Compiler (by Glenn Mark).

After your installation, turn on "Watch Sass" so that any changes in SCSS files will be updated in the CSS files.

## Main Concepts
- Variables
- Nesting
- Partial
- Mixins

### Variables
Variables store values and can be reused. 
> $primary-color: blue;
>
> p {
> &nbsp;&nbsp;&nbsp;color: $primary-color;
> }

### Nesting
Nesting gives hierarchy in CSS and, therefore, makes CSS more readable than Vanilla CSS.
>div {
>&nbsp;&nbsp;&nbsp;background-color: black;
>
> &nbsp;&nbsp;&nbsp;a {
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;text-decoration: none;
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
>
>  &nbsp;&nbsp;&nbsp;p {
>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;font-size: 25px;
>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;color: blue;
>  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
>}

### Partial
Partial - a SCSS file that contain CSS in which its variables, mixins, and functions can be used by other SCSS files via @use. A partial will be named with an underscore, like this: __partial.scss

>##### _partial.scss
>$primary-color: black;

>##### styles.scss
>@use '_partial.scss' // styles.scss can use _partial.scss's variables, mixins, and functions. 
>p {
>  color: partial.$primary-color;
>}

### Mixin
A snippet of CSS code that you can reuse. You must use "@mixins" to create the mixin, and use "@include" to use the mixin.

> ##### __partial.scss
>@mixin buttonStyle() {
>&nbsp;&nbsp;&nbsp;color: white;
>&nbsp;&nbsp;&nbsp;background-color: pink;
>}

> ##### styles.scss 
>  button {
>&nbsp;&nbsp;&nbsp;@include partial.buttonStyle;
>&nbsp;&nbsp;&nbsp;}
>


## Sources:
- https://sass-lang.com/guide