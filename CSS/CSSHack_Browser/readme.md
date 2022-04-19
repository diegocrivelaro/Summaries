# Aplicar Estilos Diferentes Para Cada Navegador

## Seletor para o IE11
```css
_:lang(x)::-ms-backdrop, body {
	background-color: #ff4081;
}
```

## Seletor para o Edge
```css
_:-ms-lang(x)::backdrop, body { background-color: #ff5252 }		
```

## Seletor para o FireFox
```css
@-mox-document url-prefix() {
	body {
		background-color: #7c4dff;
	}
}
```
```css
_:dir(x), h1 {
	color: #fff
}
```

## Seletor para o Safari
```css
_:lang(x)::x-, body {
	background-color: #64ffda
}
```

---

###### LInks
- [CSSHack 2022](https://gist.github.com/feo52/9b0658d254b0ad2333d6907e97267e5f)
- [CSSHack](https://gist.github.com/feo52/b6198873e0bbaeda098e4ca6f62ca887)
- [Descobrir o seletor para seu navegador](https://bl.ocks.org/feo52/raw/b6198873e0bbaeda098e4ca6f62ca887/)