ColorMine
=========

.Net library intended to make working with colors easy.

You can do stuff like easily convert between colors spaces like Rgb, Hsl, Xyz, Yyz, Cmy, Cmyk, and CIE*Lab. More spaces supported soon!

```c#
var startingRgb = new Rgb { R = 149, G = 13, B = 12 }
var cmy = startingColor.To<Cmy>();
```

Online example at http://colormine.org/color-converter

You can also calculate delta-e, it's currently a bit awkward but undergoing rapid development. More algorithms coming soon!

```c#
var deltaE = startingRgb.Compare(cmy,new Cie1976Comparison);
```

Online example at http://colormine.org/delta-e-calculator
