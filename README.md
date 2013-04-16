# Gridney - v0.1

Gridney is a powerful and flexible grid framework to help you build your next project easily for different devices.

To get started, clone the repository.
```
git clone https://github.com/hunab/gridney
```

Now you define what you need and Gridney does the hard work. Three simple steps to start enjoying Gridney:

1. Define some sizes of your layout (container, gutter, min-width and max-width)
2. Decide how to use Gridney: semantic or explicit (explained somewhere below)
3. If your project is responsive, choose the media queries you need from some predefined ones or create your own

@todo:

- Add mediaqueries in _mediaqueries, show a table in _config and better explanation on how to use it
- nested grids
- centered grids
- left/right proportional spaces
- extend 2 of 4 from 1 of 2
- add to .g-6of6 -> .g-all
- add to .g-1of2 -> .g-half
- Templates ready to use (examples from foundation)
- Website
- Gridney Builder (to customize everything in _config and _mediaqueries)

## What is Gridney

- Easily generate optimized grids for whatever device, nothing more, nothing less.
- Fluid or fixed, in px, em or % for the container widths, columns widths and gutter.
- Lots of predefined mediaqueries, you choose only what you need, Gridney generates only what you choose (not bloated CSS).
- Use it with SCSS or with plain CSS, so it's easy to add it to your current workflow.
- Exhaustive control of the generated CSS, every property counts.

## What is NOT Gridney

- It's not a complete UI framework. If you need styles for every element in you HTML and lot of CSS helpers, try [Bootstrap](https://github.com/twitter/bootstrap) or [Foundation](https://github.com/zurb/foundation).
- It's not a tool to build any layout with any HTML order (you can get this with flexbox), it's a grid system to use right now, in your next project with a wide browser support.

## Two ways of use it

### Semantic (using SCSS silent classes)

- @import "gridney";
- Add @gridney-container(); to your grid container
- Add @include gridney-column(1 of 3); to create your columns

### Explicit (using plain CSS)

Add classes to your html: .g, .g-1of3, .g-all...

## Advantages of inline-block + border-box:

- No need for clearfix row
- Easily horizontal alignment
- Cell dimensions are indepent from gutter/offset
- Grid nesting is efortless

## "Disadvantages" of this grid system:

- Every .g-?of? must be placed without other presentational styles if you need to style it as a boxes (because it uses padding instead of margin taking advantages of border-box sizing model).

## Requirements
- SASS 3.2+

## Browser Support

- Google Chrome (latest)
- Opera (latest)
- Firefox (latest)
- Safari (latest)
- Internet Explorer 8+

## Inspiration

- Simpletastic
- Inuit.css
- Griddle
- And many other articles
