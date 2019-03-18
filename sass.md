# Sass

## Media Queries

```scss
@mixin media768 {
  @media (min-width: 768px) {
    @content;
  }
}

@mixin media480 {
  @media (min-width: 480px) and (max-width: 767px) {
    @content;
  }
}

@mixin media320 {
  @media (min-width: 320px) and (max-width: 479px) {
    @content;
  }
}
```
