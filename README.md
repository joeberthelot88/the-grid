# The Grid

A 12x12 customizable grid built with CSS Grid and LESS.

![Grid System](http://i.imgur.com/4hh436c.png)

## Installation

Simply just clone this repo to get started! View [docs/index.html](https://joeberthelot88.github.io/Less-Grid-Boilerplate/) for a variety of different possibilities.

## Usage

The only requirements are that the columns are nested in a `.container` and a `.row`.  The markup is simple and straightforward:

```html
<div class="container">
  <div class="row">
    <div class="full">This is a full-width column.</div>
  </div>
</div>
```

## The Classes

The following classes are used to set the width of your columns:

1. .full (12/12 Columns)
2. .one-half (6/12 Columns)
3. .two-thirds (8/12 Columns)
4. .one-third (4/12 Columns)
5. .one-fourth (3/12 Columns)
6. .one-sixth (2/12 Columns)

## Helper Classes

#### Content Alignment

Aligning content is easy.  The following classes will align your content vertically and horizontally, as you wish:

1. .content-center-v (Vertically center content)
2. .content-center-h (Horizontally center content)
3. .content-end-v (Vertically align content to bottom)
4. .content-end-h (Horizontally align content to right)

Just make sure you also add the `.grid` class as well.

Example markup:

```html
<div class="container">
  <div class="row">
    <div class="full grid content-center-v content-center-h">This is a full-width column and this text is centered.</div>
  </div>
</div>
```

#### Column Alignment

1. .middle (Align a column to the middle of the grid)

Use the `.middle` class to align the column to the middle of the layout.  This only works on classes: `.one-half .two-thirds .one-third .one-sixth`.

#### Fixed Header & Footer

1. .top (Align a row to the top of the layout)
2. .bottom (Align a row to the bottom of the layout)

If you want to position an element to the top or bottom of your layout, add the `.grid` class to your `.container` and add either `.top` or `.bottom` to your `.row`.

Example markup:

```html
<div class="container grid">
  <div class="row top">
    <div class="full">Header</div>
  </div>
  <div class="row">
    <div class="two-thirds">Content</div>
    <div class="one-third">Sidebar</div>
  </div>
  <div class="row bottom">
    <div class="full">Footer</div>
  </div>
</div>
```

#### Nested Grids

Nesting grids is also extremely easy.  Just add the `.grid` class to your column and then add your inner-grid `<div>`'s inside!

Example markup:

```html
<div class="container grid">
  <div class="row">
    <div class="one-half grid">
      <div class="one-fourth">One Fourth</div>
      <div class="one-fourth">One Fourth</div>
      <div class="one-fourth">One Fourth</div>
      <div class="one-fourth">One Fourth</div>
    </div>
    <div class="one-half">One Half</div>
  </div>
</div>
```

#### Responsive Grids

Two breakpoints are provided: 768px for tablets and 576px for mobile.  Apply one of the following helper classes to your `.container` to enable column stacking:

1. .tablet-stack (Stack columns at <= 768px)
2. .mobile-stack (Stack columns at <= 576px)

To set a specific row or column to be hidden when a breakpoint is hit, just add the `.sm-hide` class.

Example markup:

```html
<div class="container mobile-stack grid">
  <div class="row">
    <div class="one-half">One Half</div>
    <div class="one-half">One Half</div>
  </div>
  <div class="row sm-hide">
    <div class="one-fourth">One Fourth</div>
    <div class="one-fourth">One Fourth</div>
    <div class="one-fourth">One Fourth</div>
    <div class="one-fourth">One Fourth</div>
  </div>
</div>
```

## Contributing

1. Fork it!
2. Create your new branch: `git checkout -b my-new-branch`
3. Commit your changes: `git commit -am 'Add some stuff'`
4. Push to the branch: `git push origin my-new-branch`
5. Submit a pull request :D

## Credits

Grid system built by Joe Berthelot.
# the-grid
