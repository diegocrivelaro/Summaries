# Animação em Borda com Hover Effect

```html
<div class="main center">
  <div class="btn center">
    <p>Clique me</p>
    <div class="d1"></div>
    <div class="d2"></div>
    <div class="d3"></div>
    <div class="d4"></div>
  </div>
</div>
```

```css
@import url("https://fonts.googleapis.com/css?family=Ubuntu&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Ubuntu", sans-serif;
}

.center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.main {
  height: 100vh;
}

.btn {
  width: 150px;
  height: 45px;
  position: relative;
  cursor: pointer;
  transition: all 0.4s;
}

.btn:hover {
  font-size: 1.2rem;
  color: white;
  transition-delay: 0.8s;
  background-color: #7b21d6;
}

.d1,
.d2 {
  position: absolute;
  width: 100%;
  height: 4px;
  background-color: #7b21d6;
  transform: scaleX(0);
  transition: all 0.4s;
  transition-delay: 0.4s;
}

.d1 {
  top: 0;
  transform-origin: left;
}

.d2 {
  bottom: 0;
  transform-origin: right;
}

.btn:hover .d1,
.btn:hover .d2 {
  transform: scaleX(1);
  transition-delay: 0s;
}

.d3,
.d4 {
  width: 4px;
  height: 100%;
  position: absolute;
  background-color: #7b21d6;
  transform: scaleY(0);
  transition: all 0.4s;
}

.d3 {
  left: 0;
  transform-origin: bottom;
}

.d4 {
  right: 0;
  transform-origin: top;
}

.btn:hover .d3,
.btn:hover .d4 {
  transform: scaleY(1);
  transition-delay: 0.4s;
}
```
