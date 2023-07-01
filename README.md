# AsciiMathToTex

Convert AsciiMath to TeX.

## Introduction

This PHP class converts [AsciiMath](http://asciimath.org/) expressions in TeX expressions. In this way [KaTeX](https://katex.org/) (which is much lighter and much faster than MathJax) can be used to render AsciiMath.

PHP >= 7.0 is required.

## Class synopsis

```php
class AsciiMathToTex {

    /* Methods */
    public __construct(string $decimalsign = ".")
    public parse(string $asciimath): string

}
```

## Example

```php
require "asciimathtotex.php";

$parser = new AsciiMathToTex();
$asciimath = "x=(-b+-sqrt(b^2-4ac))/(2a)";
$tex = $parser->parse($asciimath);
```

## Acknowledgements

This class is a translation of the original [asciimath2tex](https://github.com/christianp/asciimath2tex) by Christian Lawson-Perfect.

## Developer

Giovanni Salmeri.
