# Mavi-grid

A simple SASS customizable grid, that enables you to modify the media queries breakpoints, gutter and small gutter and the number of columns

## Install

Compile the grid.scss file and export it in a css file like "grid.css" then include it in your html:

```html
<!doctype html>
<html lang="en">
<head>
   <link rel="stylesheet" href="grid.css">
</head>
<body>
    <div class="container">
        <div class="row">
            <div class="small-12 medium-4 large-6 x-large-6">
                <p>Hello world</p>
            </div>
        </div>
        
        <div class="row">
            <div class="container-fluid">
                <p>Container fluid (column without width and float)</p>
            </div>
        </div>
        
        <div class="row">
            <div class="medium-offset-left-2 medium-5">
                <p>A 5 wide column moved two columns from left to right</p>
            </div>
        </div>
    </div>
</body>
</html>
```


### Utils


* Hidden Breakpoint Classes : hidden-{breakpoint}
* Pull Classes (floats): pull-right / pull-left
* Offset Breakpoint Classes: medium-offset-right-2 / medium-offset-left-2

### Prerequisites

```
Ruby
Sass
```


### Support

```
All browsers
IE <= 8
```

Nothing more ;)

