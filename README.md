# ECMAScript proposal: standard module uuid

Champions:  [Benjamin Coe](https://github.com/bcoe)

Status: Stage 0

***Note to contributors: this template is based on the 
[top-level await proposal](https://github.com/tc39/proposal-top-level-await), 
use this for inspiration while fleshing out document.***

## Synopsis

The standard module `@std:uuid` exposes an API for generating character
encoded Universally Unique IDentifiers (UUID), based on the IETF
[rfc4122](https://tools.ietf.org/html/rfc4122) proposal.

## Motivation

### UUID generation is an extremely common software requirement

The [uuid module](https://www.npmjs.com/package/uuid) on npm currently receives some [64,000,000 monthly downloads](https://npm-stat.com/charts.html?package=uuid) and is relied on by over
[300,000 repositories](https://libraries.io/npm/uuid).

The ubiquitous nature of the `uuid` module demonstrates that uuid generation
is a common requirement for JavaScript software applications, making the
functionality a good candidate for standard modules.

### Developers "re-inventing the wheel" is potentially harmful

Developers who have not been exposed to the rfc4122 specification (or other
vetted approaches for UUID generation) might naturally opt to invent their
own approaches to UUID generation, potentially using `Math.random()`.

It's well documented that [`Math.random()` is not cryptographically secure](https://v8.dev/blog/math-random), by instead exposing users to `@std:uuid` we prevent the pitfalls
that go hand in hand with home-grown implementations.

## Use cases

How do folks in the community use rfc4122 UUIDs?

### Creating unique keys for database entries

### Generating fake testing data

### Writing to temporary files

## FAQ

## History

## Specification

## Implementations

* none yet.

## References

* [rfc4122 proposal](https://tools.ietf.org/html/rfc4122)
* [Ecmarkup source](https://github.com/tc39/proposal-top-level-await/blob/master/spec.html)
* [HTML version](https://tc39.github.io/proposal-top-level-await/)


