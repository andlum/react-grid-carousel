<h1 style="text-align:center">React Grid Carousel</h1>
<p style="text-align:center">Flexible carousel layout w/ css grid to easily create a carousel like photo gallery, shopping product card or anything you want</p>

// TODO: badge, demo gif

## Feature

- Multi items per page
- Multi rows per page
- Infinite loop
- Support any component as a item to put into grid
- `scroll-snap` for each item on mobile device

## Install

```bash
$ npm install react-grid-carousel --save
```

## Usage

```javascript
import React from 'react'
import Carousel from 'react-grid-carousel'

const Gallery = () => {
  return (
    <Carousel cols={3} rows={3} gap={10} loop>
      <Carousel.Item>
        <img width="100%" src="https://picsum.photos/800/600?random=1" />
      </Carousel.Item>
      <Carousel.Item>
        <img width="100%" src="https://picsum.photos/800/600?random=2" />
      </Carousel.Item>
      <Carousel.Item>
        <img width="100%" src="https://picsum.photos/800/600?random=3" />
      </Carousel.Item>
      <Carousel.Item>
        {/* anything you want to show in the grid */}
      </Carousel.Item>
      {/* ... */}
    </Carousel>
  )
}
```

## Props

| Prop | Type    | Default | Description                                   |
| ---- | ------- | ------- | --------------------------------------------- |
| cols | Number  | 1       | Column amount rendered per page               |
| rows | Number  | 1       | Row amount rendered per page                  |
| gap  | Number  | 10      | Margin (grid-gap) between each item/grid (px) |
| loop | Boolean | false   | Infinite loop or not                          |

## Examples

Storybook

```bash
$ git clone https://github.com/x3388638/react-grid-carousel
$ cd react-grid-carousel
$ npm ci
$ npm run storybook
```

In actual life

```
$ npm run dev
# open localhost:8080
```

## Licence

MIT
