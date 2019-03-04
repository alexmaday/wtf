# What the Flexbox?

Notes and Observations for [the course](https://flexbox.io/) by [Wes Bos](https://twitter.com/wesbos). Additional resource at [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## The Flexible Box Model - AKA Flexbox
The attributes of flexbox are distributed through two main contexts:
1. The flex container
2. The flex items

Everything within the **flex container** now adheres to the flexible box model and all descendants of this
container become **flex items**.

To enable flexbox: `display: flex;`

## Flex container
Considerations:
* flex-direction - *main axis* (default is left-to-right)
* flex wrapping - *cross axis* (runs perpendicular to the main axis, default top-to-bottom)
* etc.

## Flex items
Considerations include:
* order
* etc.

## Alignment and Centering

### [Container attributes](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

Aligning items along the main-axis
---
| `justify-content:` | defines how items are aligned along the **main axis** and accepts <br>one of several values |
|---|---|
| `flex-start` | items are packed toward start of the line |
| `flex-end` | items are packed toward end of the line |
| `center` | items are centered along the line |
| `space-between` | items are evenly distributed in the line; first item is on the start<br> line, last item on the end line |
| `space-around` | items are evenly distributed in the line with equal space around them. <br> Note that visually the spaces aren't equal, since all the items have<br> equal space on both sides. The first item will have one unit of space<br> against the container edge, but two units of space between the next item<br> because that next item has its own spacing that applies. |
| `space-evenly` | items are distributed so that the spacing between any two items (and the<br> space to the edges) is equal. |

Aligning items along the cross-axis
---
| `align-items` | defines the default behavior for how flex items are laid out along the cross <br>axis of the current line |
|---|---|
| `stretch` | (default): stretch to fill the container (still respect min-width/max-width) |
| `flex-start` | the cross-start margin (the margin top) edge of the items is placed on the cross-start line |
| `flex-end` | cross-end margin edge of the items is placed on the cross-end line |
| `center` | items are centered in the cross-axis |
| `baseline` | items are aligned such as their baselines align |
