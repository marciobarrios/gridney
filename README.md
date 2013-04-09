# Gridney - v0.1

Gridney is a flexible grid framework to help you build your site easily for different devices.

You define what you want and Gridney does the hard work. Three simple steps to start enjoying Gridney:

1- If your project is responsive, add some mediaqueries to _mediaqueries.scss (there are lots of predefined ones)
2- Define some measures in _config.scss, choose the mediaqueries you need
3- Choose how to use Gridney: semantic or explicit

@todo:
- nested grids
- extend 2 of 4 of 1 of 2
- add to .g-6of6 -> .g-all
- add to .g-1of2 -> .g-half

Keys:
- Human-readable widths
- Fluid or fixed
- Every measure in px, em or % (gutter, width...)
- Responsive helpers
- Use it with SCSS or with plain CSS

## Config
You need to answer some simple questions in _config.scss to configure your grid system.

## Two ways of use it

### Semantic (using SCSS)

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

- Every .g-?of? must be alone without other presentational styles if you need to style it as a boxes (because it uses padding instead of margin taking advantages of border-box sizing model).

## Requirements
- If you use the semantic way, you need SASS 3.2+

## Browser Support

- Google Chrome (latest)
- Opera (latest)
- Firefox 4+
- Safari 5+
- Internet Explorer 8+

## Inspiration

- Simpletastic
- Inuit.css
- Griddle
