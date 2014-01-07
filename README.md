# lakansyèl for Stylus

> Color Scheme utilities for stylus

**lakansyèl for Stylus** is a collection of utilities to generate color schemes in your stylesheets.

## Usage

Include **lakansyèl** in your stylus stylesheets with

```css
@import "lakansyel"
```

### Utilities

#### monochrome( color )

Returns monochromatic variations of the given color.
`returned[0]`: first monochrome variation ( given color's lightness minus 33% )
`returned[1]`: second monochrome variation ( given color's lightness minus 66% )

```css
variations = monochrome( #f00 )

.red-mono-one
    color variations[0]
    
.red-mono-two
    color variations[1]
```

#### analogous( color )

Returns analogous variations of the given color.
`returned[0]`: first analogous variation ( spinning given color by 30 degrees )
`returned[1]`: second analogous variation ( spinning given color by -30 degrees )

```css
variations = analogous( #f00 )

.red-analog-one
    color variations[0]
    
.red-analog-two
    color variations[1]
```

#### extended-analogous( color )

Returns more analogous variations of the given color.
`returned[0]`: first analogous variation ( spinning given color by 30 degrees )
`returned[1]`: second analogous variation ( spinning given color by -30 degrees )
`returned[2]`: third analogous variation ( spinning given color by 60 degrees )
`returned[3]`: fourth analogous variation ( spinning given color by -60 degrees )

```css
variations = extended-analogous( #f00 )

.red-analog-one
    color variations[0]
    
.red-analog-two
    color variations[1]
    
.red-analog-three
    color variations[2]
    
.red-analog-four
    color variations[3]
```

#### split-complements( color )

Returns split-complements variations of the given color.
`returned[0]`: first split-complements variation ( spinning given color by 150 degrees )
`returned[1]`: second split-complements variation ( spinning given color by -150 degrees )

```css
variations = split-complements( #f00 )

.red-split-complement-one
    color variations[0]
    
.red-split-complement-two
    color variations[1]
```

#### triad( color )

Returns triad variations of the given color.
`returned[0]`: first triad variation ( spinning given color by 120 degrees )
`returned[1]`: second triad variation ( spinning given color by -120 degrees )

```css
variations = triad( #f00 )

.red-triad-one
    color variations[0]
    
.red-triad-two
    color variations[1]
```

#### quad( color ) & tetrad( color )

Returns quad (*tetrad*) variations of the given color.
`returned[0]`: first quad variation ( spinning given color by 90 degrees )
`returned[1]`: second quad variation ( spinning given color by -90 degrees )
`returned[2]`: third quad variation ( spinning given color by 180 degrees ) - complement color

```css
variations = quad( #f00 )

.red-quad-one
    color variations[0]
    
.red-quad-two
    color variations[1]
    
.red-quad-three
    color variations[2]
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style.  
Add unit tests for any new or changed functionality.  
Test your code using `npm test`.

## Release History

**2014-01-07** : v0.0.1

## License 

(The MIT License)

Copyright (c) 2014 Pierre-Antoine "*Leny*" Delnatte

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
