<!--

@license Apache-2.0

Copyright (c) 2019 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# Standard 52-Card Deck

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> A list of two or three letter abbreviations for each card in a standard 52-card deck.



<section class="usage">

## Usage

```javascript
import cards from 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-standard-card-deck@deno/mod.js';
```

#### cards()

Returns a list of two or three letter abbreviations for each card in a standard 52-card deck.

```javascript
var list = cards();
// returns [ 'AC', '2C', '3C', ... ]
```

Abbreviation format:

```text
<card><suit>
```

Cards: **A**, **2**, **3**, **4**, **5**, **6**, **7**, **8**, **9**, **10**, **J**, **Q**, **K**, 
where

-   `A`: ace
-   `J`: jack
-   `Q`: queen
-   `K`: king

Suit abbreviations:

-   `C`: clubs
-   `D`: diamonds
-   `H`: hearts
-   `S`: spades

</section>

<!-- /.usage -->

<section class="examples">

<!-- TODO: more creative example. -->

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import discreteUniform from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-discrete-uniform@deno/mod.js';
import cards from 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-standard-card-deck@deno/mod.js';

var list;
var len;
var idx;
var i;

list = cards();
len = list.length;

// Select random cards from the list...
for ( i = 0; i < 100; i++ ) {
    idx = discreteUniform( 0, len-1 );
    console.log( list[ idx ] );
}
```

</section>

<!-- /.examples -->



<!-- <license> -->

## License

The data files (databases) are licensed under an [Open Data Commons Public Domain Dedication & License 1.0][pddl-1.0] and their contents are licensed under [Creative Commons Zero v1.0 Universal][cc0]. The software is licensed under [Apache License, Version 2.0][apache-license].

<!-- </license> -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-standard-card-deck.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-standard-card-deck

[test-image]: https://github.com/stdlib-js/datasets-standard-card-deck/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/datasets-standard-card-deck/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/datasets-standard-card-deck/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/datasets-standard-card-deck?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/datasets-standard-card-deck.svg
[dependencies-url]: https://david-dm.org/stdlib-js/datasets-standard-card-deck/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/datasets-standard-card-deck/tree/deno
[umd-url]: https://github.com/stdlib-js/datasets-standard-card-deck/tree/umd
[esm-url]: https://github.com/stdlib-js/datasets-standard-card-deck/tree/esm

[pddl-1.0]: http://opendatacommons.org/licenses/pddl/1.0/

[cc0]: https://creativecommons.org/publicdomain/zero/1.0

[apache-license]: https://www.apache.org/licenses/LICENSE-2.0

</section>

<!-- /.links -->
