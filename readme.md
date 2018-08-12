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
### You can modify all vars

These are the default values:
```html
//Global Variables
$colNumber   : 12 !default;
$gutter      : 30 !default;
$gutterSmall : 30 !default;
$maxWidth    : 1200 !default;

//Breakpoints
$breakPoints: 4;
$small :  767  !default; // 0, 767
$medium:  768  !default; // 768, 991
$large :  992  !default; // 992, 1200
$xlarge:  1200 !default; // 1201 , X

```

You can put your own configuration if you copy these variables and put them above your import of the "grid.scss" file. In the next example we are saying to the grid to have a gutter of 20 when you are in the small breakpoint:

```html

$gutterSmall : 20;
@import "node_modules/mavi-grid/grid";

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

