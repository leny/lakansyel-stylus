# lakansyèl

> Color functions for stylus

**lakansyèl** is a collection of color functions imported from [sass](http://sass-lang.com) and [bourbon](http://bourbon.io).

## Usage

Include **lakansyèl** in your stylus stylesheets with

```css
@import "lakansyel"
```

### Functions

#### adjust_hue

```css
adjust_hue( color, degrees )
```

Changes the hue of a color. Takes a color and a number of degrees (usually between -360deg and 360deg), and returns a color with the hue rotated along the color wheel by that amount.

#### complement

```css
complement( color )
```

Returns the complement of a color. This is identical to adjust-hue(color, 180deg).

#### grayscale

```css
grayscale( color, degrees )
```

Converts a color to grayscale. This is identical to desaturate(color, 100%).

#### tint 

```css
tint( color, percent )
shade( color, percent )
```

Tint and Shade are different from `lighten()` and `darken()`.

Tint is a mix of color with white.
Shade is a mix of color with black.

Both take a color and a percent argument.
