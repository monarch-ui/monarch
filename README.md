# monarch

## layouts

Use the `#layout` class of mixins in `src/less/imports/_layouts.less` to make horizontal/vertical or grid/stack layouts.

### horizontal & vertical layouts

**Create a horizontal layout**
```css
section{
  #layout > .horizontal();
}
```

**Create a vertical layout**
```css
section{
  #layout > .vertical();
}
```

**Changing layout direction with media queries**
```css
section{
  #layout > .vertical();
}

@media all and (min-width: 50em) {
  section{
    #layout > .horizontal();
  }
}
```

### grid & stack layouts

```
section{
  #layout > .grid();
}
```

```
section{
  #layout > .stack();
}
```

**Changing between a grid and a stack with media queries**
```css
section{
  #layout > .stack();
}

@media all and (min-width: 50em) {
  section{
    #layout > .grid();
  }
}
```
