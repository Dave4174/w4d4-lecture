# Responsive Design

- What is responsive design
- Relative Units
- FlexBox
- Grid Systems
- Sass

## What is resonsive design?

- Mobile accounts for over 50% of web traffic worldwide.
- [Ref.: statista](https://www.statista.com/statistics/277125/share-of-website-traffic-coming-from-mobile-devices/)

- A multitude of different screen sizes exist across phones, "phablets," tablets, desktops, game consoles, TVs, and even wearables.
- Responsive design means that your Web app can adapt to any screen size and provide a good user-experience

## Mobile-First Design

- Create the layout for mobile first (more restrictions)
- Extend the layout for larger screen after

## View Port and Units

### View Port

- The viewport is the user's visible area of a web page.
- The viewport varies with the device, and will be smaller on a mobile phone than on a computer screen.

```html
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>What is View Port</title>
</head>
```

- A <meta> viewport element gives the browser instructions on how to control the page's dimensions and scaling.

- The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

- The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.

- [What is The Viewport?](https://www.w3schools.com/css/css_rwd_viewport.asp)

### Units

- Absolute Length Units

| Unit | Name        |
| ---- | ----------- |
| cm   | centimeters |
| mm   | milimeters  |
| in   | inches      |
| pt   | point       |
| px   | pixels      |

- Relative Length Units

| Unit | Relative to                                              |
| ---- | -------------------------------------------------------- |
| em   | Size of the parent                                  |
| rem  | Size of the root element                            |
| vw   | 1% of the viewport's width.                              |
| vh   | 1% of the viewport's height.                             |
| vmin | 1% of the viewport's smaller dimension.                  |
| vmax | 1% of the viewport's larger dimension.                   |
| %    | Percentage of the parent size (width, height, font-size) |

- [em vs rem example](https://codepen.io/DominicTremblay/pen/qBORmme)

## Floats

- [Float Example](https://codepen.io/DominicTremblay/pen/vYNgzVw)

## Flexbox

- The Flexbox Layout (Flexible Box) provides a more efficient way to lay out, align and distribute space among items in a container.

- Flex layout gives the container the ability to alter its items’ width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes).

- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

  - Main-axis / Cross-axis
  - Properties for the Flex container (parent)
  - Properties for the Flex items (children)

- [Flexbox Exercise 1](https://codepen.io/DominicTremblay/pen/ExVZWKw)

## Media-queries

- Media queries will allow you to use different CSS style rules according to various screen sizes

### Media-Query Syntax

- Max-Width

`@media only screen and (max-width: 600px) {...}`

- Min-Width

`@media only screen and (min-width: 600px) {...}`

- Both Min and Max

`@media only screen and (max-width: 600px) and (min-width: 400px) {...}`

- [Media Query Example](https://codepen.io/DominicTremblay/pen/pojReMW)

* [Media Queries for Standard Devices](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

## Grid Systems

### Bootstrap Grid System

- The Bootstrap grid system is using Flexbox

- [Bootstrap Grid](https://getbootstrap.com/docs/4.0/layout/grid/)

- Breakpoints

The Bootstrap 4 grid system has five classes:

- .col- (extra small devices - screen width less than 576px)
- .col-sm- (small devices - screen width equal to or greater than 576px)
- .col-md- (medium devices - screen width equal to or greater than 768px)
- .col-lg- (large devices - screen width equal to or greater than 992px)
- .col-xl- (xlarge devices - screen width equal to or greater than 1200px)

- [Boostrap Grid Example](https://codepen.io/DominicTremblay/pen/jObyBpy)

## SASS

- Allows for more efficient CSS
- Add features like the following:

  - Variables
  - Nesting
  - Partials
  - Mixins
  - Extend/Inheritance
  

- [Sass Demo](https://codepen.io/DominicTremblay/project/editor/ArwxLr)

- [Sass Guide](https://sass-lang.com/guide)
