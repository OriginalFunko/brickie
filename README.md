![Funko Brickie](https://raw.githubusercontent.com/OriginalFunko/brickie/master/funko-brickie.png)
# Funko Brickie

Responsive masonry layout engine for react

**demo**: coming soon.

# Setup

In the console

``yarn add @originalfunko/brickie``

-or-

``npm install @originalfunko/brickie``

# Usage

```
import Brickie from '@originalfunko/brickie'

...

// responsive
const responsiveConfig = [
  { breakpoint: 1024, columns: 3 }, 
  { breakpoint: 600, columns: 2 }, 
  { breakpoint: 480, columns: 1 } 
]

<Brickie columns={4} responsive={responsiveConfig} visibleRows={4} >
    [items]
</Brickie>

...

// with custom 'show more' button
const myButton = <button className='MY-CLASS'>go on...</button>

<Brickie columns={3} visibleRows={4} showMoreButton={myButton} >
    [items]
</Brickie>


...

// non-responsive
<Brickie columns={3} visibleRows={4} >
    [items]
</Brickie>
```

* **items**: HTML elements to arrange.
* **columns**: default number of columns
* **responsive**: array of break points, and the number of columns for that breakpoint.
* **visibleRows**: number of rows to display initially, and the number to reveal with each 'show more' click.
* **showMoreButton**: Replace the default 'show more' button.

