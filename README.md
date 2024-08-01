<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Erlang

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Erlang distribution.

<section class="installation">

## Installation

```bash
npm install @stdlib/stats-base-dists-erlang
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var erlang = require( '@stdlib/stats-base-dists-erlang' );
```

#### erlang

Erlang distribution.

```javascript
var dist = erlang;
// returns {...}
```

The namespace contains the following distribution functions:

<!-- <toc pattern="*+(cdf|pdf|mgf|quantile)*"> -->

<div class="namespace-toc">

-   <span class="signature">[`cdf( x, k, lambda )`][@stdlib/stats/base/dists/erlang/cdf]</span><span class="delimiter">: </span><span class="description">Erlang distribution cumulative distribution function.</span>
-   <span class="signature">[`logpdf( x, k, lambda )`][@stdlib/stats/base/dists/erlang/logpdf]</span><span class="delimiter">: </span><span class="description">evaluate the natural logarithm of the probability density function (PDF) for an Erlang distribution.</span>
-   <span class="signature">[`mgf( t, k, lambda )`][@stdlib/stats/base/dists/erlang/mgf]</span><span class="delimiter">: </span><span class="description">Erlang distribution moment-generating function (MGF).</span>
-   <span class="signature">[`pdf( x, k, lambda )`][@stdlib/stats/base/dists/erlang/pdf]</span><span class="delimiter">: </span><span class="description">Erlang distribution probability density function (PDF).</span>
-   <span class="signature">[`quantile( p, k, lambda )`][@stdlib/stats/base/dists/erlang/quantile]</span><span class="delimiter">: </span><span class="description">Erlang distribution quantile function.</span>

</div>

<!-- </toc> -->

The namespace contains the following functions for calculating distribution properties:

<!-- <toc pattern="*+(entropy|kurtosis|mean|median|mode|skewness|stdev|variance)*"> -->

<div class="namespace-toc">

-   <span class="signature">[`entropy( k, lambda )`][@stdlib/stats/base/dists/erlang/entropy]</span><span class="delimiter">: </span><span class="description">Erlang distribution differential entropy.</span>
-   <span class="signature">[`kurtosis( k, lambda )`][@stdlib/stats/base/dists/erlang/kurtosis]</span><span class="delimiter">: </span><span class="description">Erlang distribution excess kurtosis.</span>
-   <span class="signature">[`mean( k, lambda )`][@stdlib/stats/base/dists/erlang/mean]</span><span class="delimiter">: </span><span class="description">Erlang distribution expected value.</span>
-   <span class="signature">[`mode( k, lambda )`][@stdlib/stats/base/dists/erlang/mode]</span><span class="delimiter">: </span><span class="description">Erlang distribution mode.</span>
-   <span class="signature">[`skewness( k, lambda )`][@stdlib/stats/base/dists/erlang/skewness]</span><span class="delimiter">: </span><span class="description">Erlang distribution skewness.</span>
-   <span class="signature">[`stdev( k, lambda )`][@stdlib/stats/base/dists/erlang/stdev]</span><span class="delimiter">: </span><span class="description">Erlang distribution standard deviation.</span>
-   <span class="signature">[`variance( k, lambda )`][@stdlib/stats/base/dists/erlang/variance]</span><span class="delimiter">: </span><span class="description">Erlang distribution variance.</span>

</div>

<!-- </toc> -->

The namespace contains a constructor function for creating an [Erlang][erlang-distribution] distribution object.

<!-- <toc pattern="*ctor*"> -->

<div class="namespace-toc">

-   <span class="signature">[`Erlang( [k, lambda] )`][@stdlib/stats/base/dists/erlang/ctor]</span><span class="delimiter">: </span><span class="description">Erlang distribution constructor.</span>

</div>

<!-- </toc> -->

```javascript
var Erlang = require( '@stdlib/stats-base-dists-erlang' ).Erlang;

var dist = new Erlang( 2, 4.0 );

var y = dist.logpdf( 0.8 );
// returns ~-0.65
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils-keys' );
var erlang = require( '@stdlib/stats-base-dists-erlang' );

console.log( objectKeys( erlang ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/stats-base-dists-erlang.svg
[npm-url]: https://npmjs.org/package/@stdlib/stats-base-dists-erlang

[test-image]: https://github.com/stdlib-js/stats-base-dists-erlang/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/stats-base-dists-erlang/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/stats-base-dists-erlang/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/stats-base-dists-erlang?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/stats-base-dists-erlang.svg
[dependencies-url]: https://david-dm.org/stdlib-js/stats-base-dists-erlang/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/stats-base-dists-erlang/tree/deno
[deno-readme]: https://github.com/stdlib-js/stats-base-dists-erlang/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/stats-base-dists-erlang/tree/umd
[umd-readme]: https://github.com/stdlib-js/stats-base-dists-erlang/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/stats-base-dists-erlang/tree/esm
[esm-readme]: https://github.com/stdlib-js/stats-base-dists-erlang/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/stats-base-dists-erlang/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/stats-base-dists-erlang/main/LICENSE

[erlang-distribution]: https://en.wikipedia.org/wiki/Erlang_distribution

<!-- <toc-links> -->

[@stdlib/stats/base/dists/erlang/ctor]: https://github.com/stdlib-js/stats-base-dists-erlang-ctor

[@stdlib/stats/base/dists/erlang/entropy]: https://github.com/stdlib-js/stats-base-dists-erlang-entropy

[@stdlib/stats/base/dists/erlang/kurtosis]: https://github.com/stdlib-js/stats-base-dists-erlang-kurtosis

[@stdlib/stats/base/dists/erlang/mean]: https://github.com/stdlib-js/stats-base-dists-erlang-mean

[@stdlib/stats/base/dists/erlang/mode]: https://github.com/stdlib-js/stats-base-dists-erlang-mode

[@stdlib/stats/base/dists/erlang/skewness]: https://github.com/stdlib-js/stats-base-dists-erlang-skewness

[@stdlib/stats/base/dists/erlang/stdev]: https://github.com/stdlib-js/stats-base-dists-erlang-stdev

[@stdlib/stats/base/dists/erlang/variance]: https://github.com/stdlib-js/stats-base-dists-erlang-variance

[@stdlib/stats/base/dists/erlang/cdf]: https://github.com/stdlib-js/stats-base-dists-erlang-cdf

[@stdlib/stats/base/dists/erlang/logpdf]: https://github.com/stdlib-js/stats-base-dists-erlang-logpdf

[@stdlib/stats/base/dists/erlang/mgf]: https://github.com/stdlib-js/stats-base-dists-erlang-mgf

[@stdlib/stats/base/dists/erlang/pdf]: https://github.com/stdlib-js/stats-base-dists-erlang-pdf

[@stdlib/stats/base/dists/erlang/quantile]: https://github.com/stdlib-js/stats-base-dists-erlang-quantile

<!-- </toc-links> -->

</section>

<!-- /.links -->
