# Liquid Grid SASS Plugin

Liquid Grid is a minimalist and scalable SCSS mixin that generates a responsive grid and is less than <2kb out of the box.

Add liquid settings into your desired file. I recommend using a _variables.scss file for this.

## Usage

#### Setup

```scss
@import "liquid-grid.scss";

$grid-columns: 12;
$grid-gap: 56px;
$full-width-breakpoint: 768px;

@include liquid-grid($grid-columns, $grid-gap, $full-width-breakpoint)
```

#### Generating classes
Liquid grid automatically generates classes for you. They can be used in the following way:

```scss
@include liquid-grid($grid-columns, $grid-gap, $full-width-breakpoint)

// Outputs classes based on the your settings params. 
// By default, it outputs grid and grid modifier classes as well as 12 column classes:
//
// Grid Classes
// .grid // grid wrapper
// .grid--no-responsive // disable full width responsive
// .grid--no-gutters // disables gutters
//
// Column Classes
// .col // flexible column width
// .col-1 // 8.33% column width
// .col-2 // 16.66% column width
// .col-3 // 25% column width
// .col-4 // 33.33% column width
// .col-5 // 41.66% column width
// .col-6 // 50% column width
// .col-7 // 58.33% column width
// .col-8 // 66.66% column width
// .col-9 // 75% column width
// .col-10 // 83.33% column width
// .col-11 // 91.66% column width
// .col-12 // 100% column width
```
