# kotest-extensions-arrow

Kotest extension for [Arrow](https://arrow-kt.io/).

See [docs](https://kotest.io/docs/assertions/arrow.html).

Please create issues on the main kotest [board](https://github.com/kotest/kotest/issues).

[![Build Status](https://github.com/kotest/kotest-extensions-arrow/workflows/master/badge.svg)](https://github.com/kotest/kotest-extensions-arrow/actions)
[<img src="https://img.shields.io/maven-central/v/io.kotest.extensions/kotest-assertions-arrow.svg?label=latest%20release"/>](http://search.maven.org/#search|ga|1|kotest-assertions-arrow)
![GitHub](https://img.shields.io/github/license/kotest/kotest-extensions-arrow)
[![kotest @ kotlinlang.slack.com](https://img.shields.io/static/v1?label=kotlinlang&message=kotest&color=blue&logo=slack)](https://kotlinlang.slack.com/archives/CT0G9SD7Z)
[<img src="https://img.shields.io/nexus/s/https/oss.sonatype.org/io.kotest.extensions/kotest-assertions-arrow.svg?label=latest%20snapshot"/>](https://oss.sonatype.org/content/repositories/snapshots/io/kotest/extensions/kotest-assertions-arrow/)

## Changelog

### 1.1.0
* Update to Arrow 1.0.0
* fix Java 1.8 compatibility [#2437](https://github.com/kotest/kotest/issues/2437)
* Added `kotest-property-arrow` and `kotest-property-arrow-optics` for property-based testing with Arrow
* includes deprecation cycle of 1.0.3
* remove dependency to kotlinX-coroutines and kotest-property in `kotest-assertions-arrow`

### 1.0.3
* Update to Arrow 0.13.2
* Added a deprecation cycle for previous descriptors in 1.0.2 in favor of smart-casted variants in `io.kotest.assertions.arrow.core`
* Reorg existing functions to `io.kotest.assertions.arrow.core`
* Not leaking the arrow dependency into the runtime of users
* Added Arb<Either<A, B>, Arb<Validated<E, A>>

### 1.0.2
* Updated to arrow 0.13.1
* Updated option to support nullables
