# AsciiMathToTex

Convert AsciiMath to TeX.

## Purpose

This PHP class converts [AsciiMath]http://asciimath.org/() expressions in TeX expressions. In this way [KaTeX](https://katex.org/) (which is much lighter and much faster than MathJax) can be used to render AsciiMath.

PHP >= 7.0 is required.

## Methods

The class `AsciiMathToTex` gives access to the API. The following method is available:

`parse($asciimath): string`  
Convert an AsciiMath expression in a TeX expression

## Example

```php
require "asciimathtotex.php";

$parser = new AsciiMathToTex("."); // the argument is the decimal sign
$asciimath = "x=(-b+-sqrt(b^2-4ac))/(2a)";
$tex = $parser->parse($asciimath);
```

## Acknowledgements

This class is a translation of the original [asciimath2tex](https://github.com/christianp/asciimath2tex) by Christian Lawson-Perfect.

## Developer

Giovanni Salmeri.
