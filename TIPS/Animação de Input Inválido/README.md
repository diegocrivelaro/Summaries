# Animação de input

- Animação de valores errados sendo inseridos no input

```html
<input type="text" pattern="[a-z]*" />
```

```css
* {
  outline: 0;
}

input:invalid {
  border: 2px solid red;
  border-radius: 8px;
  animation: snake 300ms;
}

@keyframes snake {
  0% {
    transform: translateX(4px);
  }
  50% {
    transform: translateX(-4px);
  }
  75% {
    transform: translateX(4px);
  }
}
```
