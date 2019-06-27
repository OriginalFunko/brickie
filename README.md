![Funko Brickie](https://raw.githubusercontent.com/OriginalFunko/brickie/master/funko-brickie.png)
# Funko Brickie
[![License: MPL 2.0](https://img.shields.io/npm/l/@originalfunko/brickie.svg?color=rgb%2868%2C%20204%2C%2017%29)](https://opensource.org/licenses/MPL-2.0)
[![minZip size](https://img.shields.io/bundlephobia/minzip/@originalfunko/brickie@0.0.3.svg?color=rgb%2868%2C%20204%2C%2017%29)](https://bundlephobia.com/result?p=@originalfunko/brickie@0.0.3)
![GitHub issues](https://img.shields.io/github/issues/originalfunko/brickie.svg?color=rgb%2868%2C%20204%2C%2017%29)
![npm](https://img.shields.io/npm/v/@originalfunko/brickie.svg?color=rgb%2868%2C%20204%2C%2017%29)

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

