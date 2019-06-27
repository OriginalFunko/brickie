# Funko Brickie

Responsive masonry layout engine for react

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

<Brickie columns={3} responsive={responsiveConfig} >
    [items]
</Brickie>

...

// non-responsive
<Brickie columns={3} >
    [items]
</Brickie>
```
