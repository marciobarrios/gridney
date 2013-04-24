# Gridney - v0.1 (In progress)

Gridney is a flexible grid framework to help you build your site easily for different devices.

What is Gridney:

- Easily generate optimized grids for whatever device; nothing more, nothing less.
- Fluid or fixed, in px, em or % for the containers, column widths and gutters.
- Lots of predefined mediaqueries, you choose only what you need, and Gridney generates only what you choose (not bloated CSS).
- Built with SASS, so you can use it with SCSS or with plain CSS, it's easy to add it to your current workflow.
- Exhaustive control of the generated CSS, every property counts.

What is NOT Gridney:

- It's not a complete UI framework. If you need styles for every element in you HTML and lot of CSS helpers, try [Bootstrap](https://github.com/twitter/bootstrap) or [Foundation](https://github.com/zurb/foundation).
- It's not a tool to build any layout with any HTML order (what you can get with [flexbox](https://developer.mozilla.org/en-US/docs/CSS/Tutorials/Using_CSS_flexible_boxes)), it's a grid system to use right now, in your next project with a wide browser support.

Gridney uses inline-block + border-box to provide these grid features:

- No need for clearfix row
- Easily horizontal alignment
- Cell dimensions are indepent from gutter/offset
- Grid nesting is efortless

"Disadvantages" of this grid system:

- Every .g-?of? must be placed without other presentational styles if you need to style it as a boxes (because it uses padding instead of margin taking advantages of border-box sizing model).

# Installation

First of all be sure you have installed at least **SASS 3.2+**

Via command line

  $ git clone https://github.com/hunab/gridney
  $ cd gridney && sh compile.sh

Now you define what you need and Gridney does the hard work. Three simple steps to start enjoying Gridney:

1. Define some sizes of your layout (container, gutter, min-width and max-width)
2. Decide how to use Gridney: semantic or explicit (explained just below)
3. If your project is responsive, choose the media queries you need from some predefined ones or create your own

## Two ways of use it

### Semantic (using SCSS silent classes)

- @import "gridney";
- Add @gridney-container(); to your grid container
- Add @include gridney-column(1 of 3); to create your columns

### Explicit (using plain CSS)

Add classes to your html: .g, .g-1of3, .g-all...

## Browser Support

- Google Chrome (latest)
- Opera (latest)
- Firefox (latest)
- Safari (latest)
- Internet Explorer 8+

## Inspiration

- Nicolle Sullivan
- Nicollas Gallagher
- Simpletastic
- Inuit.css
- Griddle
- And many other articles and people...
