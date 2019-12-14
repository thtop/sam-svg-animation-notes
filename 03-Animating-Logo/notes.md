## SVG Project - Animating a Logo

### Introductions to Project

---

### Drawing The SVG

---

### Create Line Animations

```css
svg {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
}

.square {
  stroke-dasharray: 650;
  stroke-dashoffset: -650;
  animation: draw-square 1s infinite;
}

@keyframes draw-square {
  from {
    stroke-dashoffset: -650;
  }

  to {
    stroke-dashoffset: 0;
  }
}
```

---

### JavaScript Line Calculation

```js
// const shape = document.querySelector(".square");
const shape = document.querySelector(".hexagon");
const shapeLenght = shape.getTotalLength();
console.log(shapeLenght);
```

---

### Add Final Animations

```css
svg {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  margin: auto;
}

.square {
  stroke-dasharray: 650;
  stroke-dashoffset: -650;
  animation: draw-square 2s infinite;
  transform-origin: 50% 50%;
}

@keyframes draw-square {
  from {
    stroke-dashoffset: -650;
    transform: rotate(0deg);
  }

  to {
    stroke-dashoffset: 0;
    transform: rotate(720deg);
  }
}

.hexagon {
  stroke-dasharray: 425;
  stroke-dashoffset: -425;
  animation: draw-hexagon 2s infinite;
  transform-origin: 50% 50%;
}

@keyframes draw-hexagon {
  from {
    stroke-dashoffset: -425;
    transform: rotate(0deg);
  }

  to {
    stroke-dashoffset: 0;
    transform: rotate(360deg);
  }
}
```
