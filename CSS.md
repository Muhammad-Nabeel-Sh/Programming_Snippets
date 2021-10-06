# CSS Snippets

## Background Styles

```CSS
element {
  background-color: color|transparent|initial|inherit;
  background-image: url("")|none|initial|inherit;
  background-origin: ;
  background-position: ;
  background-position-x: ;
  background-position-y: ;
  background-repeat: repeat|repeat-x|repeat-y|no-repeat|initial|inherit ;
  background-clip: border-box|padding-box|content-box|initial|inherit ;
  background-attachment: scroll|fixed|local|initial|inherit ;
  backdrop-filter: ;
  background-blend-mode: normal|multiply|screen|overlay|darken|lighten|color-dodge|saturation|color|luminosity ;
  background: bg-color bg-image position/bg-size bg-repeat bg-origin bg-clip bg-attachment initial|inherit;
```

## Colors

| Color names | Hexadecimal | Hex with Aplha |       RGB        |        RGBA         |         HSL         |          HSLA          |
| :---------: | :---------: | :------------: | :--------------: | :-----------------: | :-----------------: | :--------------------: |
|     Red     |  \#ff0000   |   \#ff0000ff   |  rgb\(255,0,0\)  |  rgba\(255,0,0,1\)  |  hsl\(0,100%,50%\)  |  hsla\(0,100%,50%,1\)  |
|    Green    |  \#00ff00   |   \#00ff00ff   |  rgb\(0,255,0\)  |  rgba\(0,255,0,1\)  | hsl\(120,100%,50%\) | hsla\(120,100%,50%,1\) |
|    Blue     |  \#0000ff   |   \#0000ffff   |  rgb\(0,0,255\)  |  rgba\(0,0,255,1\)  | hsl\(240,100%,50%\) | hsla\(240,100%,50%,1\) |
|   Magenta   |  \#ff00ff   |   \#ff00ffff   | rgb\(255,0,255\) | rgba\(255,0,255,1\) | hsl\(300,100%,50%\) | hsla\(300,100%,50%,1\) |
|    Cyan     |  \#00ffff   |   \#00ffffff   | rgb\(0,255,255\) | rgba\(0,255,255,1\) | hsl\(180,100%,50%\) | hsla\(180,100%,50%,1\) |
|   Yellow    |  \#ffff00   |   \#ffff00ff   | rgb\(255,255,0\) | rgba\(255,255,0,1\) | hsl\(60,100%,50%\)  | hsla\(60,100%,50%,1\)  |


```CSS
element {color: #ff00ff; } /* Hexadecimal notation #rrggbb */
element {color: #f0f; }
element {color: #rrggbbaa; } /* Hexadecimal notation with alpha channel #rrggbbaa */
element {color: rgb(255,0,255); } /* RGB function rgb(red,green,blue) */
element {color: rgba(255,0,255,1); } /* RGB function with alpha channel rgba(red,green,blue,alpha) */ 
element {color: hsl(300,100%,50%); } /* HSL function hsl(hue,saturation,lightness) */
element {color: hsla(300,100%,50%); } /* HSLA function hsla(hue,saturation,lightness,alpha) */
element {background-image: linear-gradient(direction, color-stop1, color-stop2, ...); } /* to bottom, to top, to right, to left, to bottom right, etc. */
element {background-image: linear-gradient(to right, rgba(255,0,0,0), rgba(255,0,0,1)); }
element {background-image: repeating-linear-gradient(angle | to side-or-corner, color-stop1, color-stop2, ...); }
element {background-image: radial-gradient(shape size at position, start-color, ..., last-color); }
element {background-image: repeating-radial-gradient(shape size at position, start-color, ..., last-color); }
```

### Alpha Channel to Hex Code

```js
const percentToHex = (p) => {
    const percent = Math.max(0, Math.min(100, p)); // bound percent from 0 to 100
    const intValue = Math.round(p / 100 * 255); // map percent to nearest integer (0 - 255)
    const hexValue = intValue.toString(16); // get hexadecimal representation
    return hexValue.padStart(2, '0').toUpperCase(); // format with leading 0 and upper case characters
}

console.log(percentToHex(0)); // 00
console.log(percentToHex(50)); // 80
console.log(percentToHex(80)); // CC
console.log(percentToHex(100)); // FF
```

## Layout and Box Model

### Positioning

- Static: positioned according to the normal flow of the document.
- Absolute: The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial containing block. 
- Fixed: positioned relative to the viewport.
- Relative: positioned relative to its normal position. The element is positioned according to the normal flow of the document, and then offset relative to itself based on the values of `top`, `right`, `bottom`, and `left`. The offset does not affect the position of any other elements; thus, the space given for the element in the page layout is the same as if position were static.
- Sticky: A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position:fixed).
- Z-index: specifies the stack order of an element


```CSS
element {
  position: static|absolute|fixed|relative|sticky|initial|inherit ;
  top: ;
  bottom: ;
  right: ;
  left: ;
  z-index: ;}
  ```


```CSS
element{
  padding-top: ;
  padding-bottom: ;
  padding-left: ;
  padding-right: ;
  padding: ;
  padding-inline-start: ;
  padding-inline-end: ;
  padding-inline: ;
  padding-block-start: ;
  padding-block-end: ;
  padding-block: ;

  border-top: ;
  border-bottom: ;
  border-left: ;
  border-right: ;
  border: ;

  border-bottom-left-radius: ;
  border-bottom-right-radius: ;
  border-top-left-radius: ;
  border-top-right-radius: ;
  border-radius: ;

  border-top-color: ;
  border-bottom-color: ;
  border-left-color: ;
  border-right-color: ;
  border-color: ;

  border-style: ;
  border-top-style: ;
  border-bottom-style: ;
  border-left-style: ;
  border-right-style: ;

  border-top-width: ;
  border-bottom-width: ;
  border-left-width: ;
  border-right-width: ;

  border-collapse: ;
  border-spacing: ;
  border-image: ;

  outline: outline-width outline-style outline-color|initial|inherit;
  outline-color: invert|color|initial|inherit;
  outline-offset: length|initial|inherit;
  outline-style: none|hidden|dotted|dashed|solid|double|groove|ridge|inset|outset|initial|inherit;
  outline-width: medium|thin|thick|length|initial|inherit;

  margin-top: ;
  margin-bottom: ;
  margin-left: ;
  margin-right: ;
  margin: ;
  margin-inline-start: ;
  margin-inline-end: ;
  margin-inline: ;
  margin-block-start: ;
  margin-block-end: ;
  margin-block: ;
  margin-trim: ;
}
```

## Flexbox

```CSS
Parent {
  display: flex;
  flex-direction: row|row-reverse|column|column-reverse|initial|inherit ;
  flex-wrap: nowrap|wrap|wrap-reverse|initial|inherit ;
  flex-flow: flex-direction flex-wrap|initial|inherit ;
  flex-grow: ;
  flex-shrink: ;
  flex-basis: ;
  flex: ;
  justify-content: flex-start|flex-end|center|space-between|space-around|space-evenly|initial|inherit ;
  justify-items: ;
  align-items: stretch|center|flex-start|flex-end|baseline|initial|inherit ;
  align-content: stretch|center|flex-start|flex-end|space-between|space-around|initial|inherit ;
}

Child {
  align-self: auto|stretch|center|flex-start|flex-end|baseline|initial|inherit ;
  justify-self: ;
  flex-grow: ;
  flex-shrink: ;
  flex-basis: ;
  flex: flex-grow flex-shrink flex-basis|auto|initial|inherit ;
  order: ;
}
```
## Grid

```CSS
Parent {
  display: grid;
  grid-template-columns: ;
  grid-column: ;
  grid-template-rows: ;
  grid-row: ;
  grid-template-areas: ;
  grid-template: ;

  grid-column-gap: ;
  grid-row-gap: ;
  grid-gap: ;

  grid-column-start: ;
  grid-column-end: ;
  grid-row-start: ;
  grid-row-end: ;

  grid-auto-columns: ;
  grid-auto-rows: ;
  grid-auto-flow: ;

  justify-content: flex-start|flex-end|center|space-between|space-around|space-evenly|initial|inherit ;
  justify-items: ;
  justify-tracks: ;
  align-items: stretch|center|flex-start|flex-end|baseline|initial|inherit ;
  align-content: stretch|center|flex-start|flex-end|space-between|space-around|initial|inherit ;
}

Child {
  grid-area: ;
  align-self: auto|stretch|center|flex-start|flex-end|baseline|initial|inherit ;
  justify-self: ;
  place-self: ;
}
```

## Scrollbars

```CSS
html {
  scroll-behavior: smooth;
}

/* the scrollbar. */
::-webkit-scrollbar {
  width: ;
}

/*the buttons on the scrollbar (arrows pointing upwards and downwards).*/
::-webkit-scrollbar-button  {
}

/*the draggable scrolling handle.*/
::-webkit-scrollbar-thumb  {
}

/*the track (progress bar) of the scrollbar.*/
::-webkit-scrollbar-track {
}

/*the track (progress bar) NOT covered by the handle.*/
::-webkit-scrollbar-track-piece {
}

/*the bottom corner of the scrollbar, where both horizontal and vertical scrollbars meet.*/
::-webkit-scrollbar-corner {
}

/*the draggable resizing handle that appears at the bottom corner of some elements.*/
::-webkit-resizer {
}
```
### Scroll Snap
```CSS
Parent {
  scroll-snap-type: y mandatory;
  overflow-y: scroll;
}

Child {
  scroll-snap-align: start;
}
```

## Tables

```CSS
table {
  width: ;
  height: ;
  border: ;
  border-bottom: ; /*Horizontal dividers*/
  border-radius: ;
  border-collapse: separate|collapse|initial|inherit ;
  border-style: ;
  border-spacing: ;
  text-align: ;
  vertical-align: ;
  white-space: ;
  table-layout: ;
  empty-cells: show|hide|initial|inherit ;
}

td:hover,
th:hover {
  background-color: ;
}

/*Zebra Stripes*/
tr:nth-child(even) {
  background-color: ; 
}
tr:nth-child(odd) {
  background-color: ;
}

/*Column Highlight*/
tr:nth-child(n) {
  background-color: ;
}

caption {
  caption-side: ;
  text-align: ;
}
```

## Text

```CSS
element{
  font: ;
  font-family: family-name|generic-family|initial|inherit;
  font-size: medium|xx-small|x-small|small|large|x-large|xx-large|smaller|larger|length|initial|inherit;
  font-weight: normal|bold|bolder|lighter|number|initial|inherit;
  font-style: normal|italic|oblique|initial|inherit;
  font-variant: normal|small-caps|initial|inherit;
  font-display: ;
  font-stretch: ultra-condensed|extra-condensed|condensed|semi-condensed|normal|semi-expanded|expanded|extra-expanded|ultra-expanded|initial|inherit;
  font-kerning: auto|normal|none;
  font-synthesis: ;
  
  text-decoration: text-decoration-line text-decoration-color text-decoration-style|initial|inherit ;
  text-decoration-color: ;
  text-decoration-skip: ;
  text-decoration-line: none|underline|overline|line-through|initial|inherit ;
  text-decoration-style: solid|double|dotted|dashed|wavy|initial|inherit ;
  text-decoration-thickness: ;
  text-decoration-skip-ink: ;
  text-underline-offset: ;
  text-underline-position: ;

  text-transform: none|capitalize|uppercase|lowercase|initial|inherit ;
  text-overflow: ;
  text-orientation: ;
  text-emphasis: ;
  text-emphasis-color: ;
  text-emphasis-position: ;
  text-emphasis-style: ;

  text-shadow: h-shadow v-shadow blur-radius color|none|initial|inherit;
  text-anchor: ;

  direction: ltr|rtl|initial|inherit;
  writing-mode: horizontal-tb|vertical-rl|vertical-lr;
  unicode-bidi: normal|embed|isolate|bidi-override|isolate-override|plaintext|inherit|initial|revert|unset;

  text-align: left|right|center|justify|initial|inherit ;
  text-align-last: auto|left|right|center|justify|start|end|initial|inherit;
  text-indent: ;
  vertical-align: baseline|length|sub|super|top|text-top|middle|bottom|text-bottom|initial|inherit;
  hyphens: none|manual|auto|inherit|initial|revert|unset;
  hanging-punctuation: none|first|last|force-end|allow-end|inherit|initial|revert|unset;

  white-space: normal|nowrap|pre|pre-line|pre-wrap|initial|inherit;
  word-wrap: normal|break-word|initial|inherit;
  word-break: normal|break-all|keep-all|break-word|initial|inherit;
  word-spacing: normal|length|initial|inherit;
  letter-spacing: normal|length|initial|inherit;
  line-height: normal|number|length|initial|inherit;
  line-break: auto|loose|normal|strict|anywhere|inherit|initial|revert|unset;
}
```

## List

```CSS
element{
  list-style-type: ;
  list-style-position: ;
  list-style-image: ;
  list-style: ;
}
```