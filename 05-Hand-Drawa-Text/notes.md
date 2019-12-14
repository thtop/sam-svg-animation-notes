## Hand Drawn Text Animation Project

### Create SVG Text

### Animation Text Writing Effect

```js
const path = document.querySelector("path");
const pathLength = path.getTotalLength();
console.log(pathLength); //562.3710327148438
```

```css
path {
  stroke-dasharray: 563;
  animation: draw 2s reverse infinite;
}

@keyframes draw {
  from {
    stroke-dashoffset: 0;
  }
  to {
    stroke-dashoffset: 563;
  }
}
```
