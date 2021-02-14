# p5.js Math

This folder contains modules with math functions.

## [calculation.js](./calculation.js)

General mathematical functions, like `sqrt()` (square root), `ceil()` (round to next highest integer), `floor()` (round to next lowest integer), etc.

## [math.js](./math.js)

Contains `createVector()`.

## [noise.js](./math.js)

Contains functions relating to [Perlin noise](https://natureofcode.com/book/introduction/#i6-perlin-noise-a-smoother-approach), which produces a "smooth" gradient of pseudo-random numbers along multiple dimensions. `noise()`, `noiseDetail()` and `noiseSeed()`.

## [p5.Vector.js](./p5.Vector.js)

Vector functions. Should include mutable and static versions.

Mutable functions modify the value of the original vector that they operate on:

```
let v = new p5.Vector(10, 0, 0);
v.normalize();
print(v); // [1, 0, 0]
```

Static functions return the new value but leave the original unchanged:

```
const v0 = new p5.Vector(10, 0, 0);
const v1 = v0.normalize();
print(v0); // [10, 0, 0] <- unchanged
print(v1); // [1, 0, 0] <- normalized
```

## [random.js](./random.js)

Includes functions for obtaining a random item from an array, number from a seeded Linear Congruential Generator (`random()`) or based on a Gaussian distribution (`randomGaussian()`).

## [trigonometry.js](./trigonometry.js)

Contains trigonometric functions and the angleMode state.