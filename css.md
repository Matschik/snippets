# CSS

## Better font rendering
```css
p {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
```

## UL reset
```css
ul {
  list-style-type: none;
  padding-left: 0px;
  margin-top: 0px;
  margin-bottom: 0px;
}
```

## Layout

## Layout container
```css
.layout:after {
  clear: both;
  content: "";
  display: table;
}
```

## Layout columns
```css
.layout-4c {
  float: left;
  width: 24.25%;
}

.layout-3c {
  float: left;
  width: 33.33%;
}

.layout-2c {
  float: left;
  width: 50%;
}
```
/* Dynamic columns */
```css
/* one column */
.layout-dc:first-child:nth-last-child(1) {
  float: left;
  width: 100%;
}

/* two columns */
.layout-dc:first-child:nth-last-child(2),
.layout-dc:first-child:nth-last-child(2) ~ .layout-dc {
  float: left;
  width: 50%;
}

/* three columns */
.layout-dc:first-child:nth-last-child(3),
.layout-dc:first-child:nth-last-child(3) ~ .layout-dc {
  float: left;
  width: 33.3333%;
}

/* four columns */
.layout-dc:first-child:nth-last-child(4),
.layout-dc:first-child:nth-last-child(4) ~ .layout-dc {
  float: left;
  width: 25%;
}
```


/* Link reset */
```css
a {
  color: inherit;
  text-decoration: none;
}
```

## Font face
```css
@font-face {
  font-family: 'MyWebFont';
  src: url('webfont.eot'); /* IE9 Compat Modes */
  src: url('webfont.eot?#iefix') format('embedded-opentype'), /* IE6-IE8 */
       url('webfont.woff2') format('woff2'), /* Super Modern Browsers */
       url('webfont.woff') format('woff'), /* Pretty Modern Browsers */
       url('webfont.ttf')  format('truetype'), /* Safari, Android, iOS */
       url('webfont.svg#svgFontName') format('svg'); /* Legacy iOS */
}
```

## Icon via data-icon
```css
.icon:before {
  content: attr(data-icon);
}
```

## Delay style
```css
div{
    -webkit-transition: 0s background-color;
    -o-transition: 0s background-color;
    transition: 0s background-color;
}

div:hover{
    background-color:red;    
    -webkit-transition-delay:1s;    
         -o-transition-delay:1s;    
            transition-delay:1s;
}
```
