## max-width?

https://developer.mozilla.org/en-US/docs/Web/CSS/min

**as-is**

```css
.container {
  width: 800%;
  max-width: 90%;
}
```

**to-be**

```css
.container {
  width: min(800px, 90%);
}
```

## min-width and max-width

**as-is**

```css
.container {
  width: 50vw;
  min-width: 400px;
  max-width: 800px;
}
```

**to-be**

`clamp(min, preferred, max)`

```css
.container {
  width: clamp(400px, 50vw, 800px);
}
```

## text gradient

```css
.gradient-text {
  color: transparent;
  background: linear-gradient(to right, red, blue);
  background-clip: text;
}
```
