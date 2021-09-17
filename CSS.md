# CSS Snippets

## Background Styles

```CSS
element {
  background-image: url("");
  background-origin: ;
  background-position: ;
  background-position-x: ;
  background-position-y: ;
  background-repeat: repeat|repeat-x|repeat-y|no-repeat|initial|inherit ;
  background-clip: border-box|padding-box|content-box|initial|inherit ;
  background-attachment: scroll|fixed|local|initial|inherit ;
  backdrop-filter: ;
  background-blend-mode: normal|multiply|screen|overlay|darken|lighten|color-dodge|saturation|color|luminosity ;
```

## Box Model

```CSS
element {
  position: static|absolute|fixed|relative|sticky|initial|inherit ;
  top: ;
  bottom: ;
  right: ;
  left: ;
  z-index: ; */

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
  font-family: ;
  font-size: ;
  font-weight: ;
  font-style: ;
  font-variant: ;
  font-display: ;
  font-stretch: ;
  font-kerning: ;
  font-synthesis: ; */
  
  text-align: left|right|center|justify|initial|inherit ;
  text-decoration: text-decoration-line text-decoration-color text-decoration-style|initial|inherit ;
  text-decoration-color: ;
  text-decoration-skip: ;
  text-decoration-line: none|underline|overline|line-through|initial|inherit ;
  text-decoration-style: solid|double|dotted|dashed|wavy|initial|inherit ;
  text-decoration-thickness: ;
  text-decoration-skip-ink: ;
  text-transform: none|capitalize|uppercase|lowercase|initial|inherit ;
  text-overflow: ;
  text-indent: ;
  text-orientation: ;
  text-emphasis: ;
  text-emphasis-color: ;
  text-emphasis-position: ;
  text-emphasis-style: ;
  text-underline-offset: ;
  text-underline-position: ;
  text-shadow: ;
  text-anchor: ;
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