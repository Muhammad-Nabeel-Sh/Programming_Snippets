# CSS Hacks

## Center a div Horizontally and Vertically
```CSS
div {
  position: absolute;
  top: 50%;
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}
```