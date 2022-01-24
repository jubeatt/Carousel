# Carousel

My first module!

## How to Install

Just clone this repository：

```bash
git clone https://github.com/jubeatt/Carousel
```

and you'll get these two files：

- carousel.js
- carousel.css


## How to use

Paste this code to into your HTML：

```html
<div class="carousel">
  <div class="carousel__container">
    <div class="carousel__item"><img src="yourImage"></div>
    <div class="carousel__item"><img src="yourImage"></div>
    <div class="carousel__item"><img src="yourImage"></div>
    <div class="carousel__item"><img src="yourImage"></div>
  </div>
  <div class="carousel__buttons-block"></div>
  <button class="carousel__prev-button fas fa-chevron-left"></button>
  <button class="carousel__next-button fas fa-chevron-right"></button>
</div>
```

and CSS file, font-awesome [CDN](https://cdnjs.com/libraries/font-awesome/4.7.0)：

```html
<!-- carousel.css -->
<link rel="stylesheet" href="carousel.css">
<!-- font-awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" integrity="sha512-1ycn6IcaQQ40/MKBW2W4Rhis/DbILU74C1vSrLJxCq57o941Ym01SwNsOMqvEBFlcgUa6xLiPY/NS5R+E6ztJQ==" crossorigin="anonymous" referrerpolicy="no-referrer" />
```

In the end, import the module from carousel.js：

```js
<script type="module">
  import { createCarousel } from './carousel.js'
  createCarousel({width: 0.8, height: 500, isLoop: false})
</script>
```


## Demo

![carousel](carousel.gif)



[Live demo](https://jubeatt.github.io/Carousel/)

## Options

| Params     | type | value      | default  |
|--------|--------|------------|------------ |
| width | Number    | `0.0` ~ `1.0` | `width: 0.8` |
| height | Number  |  `0` ~ `1000`  | `height: 500` |
| isLoop   | Boolean   | `true` / `false` | `lsLoop: false` |


The `width` will refers to the viewport：

- `0.5` will set the carousel width 50% from the viewport
- `0.8` will set the carousel width 80% from the viewport
- and so on


