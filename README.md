# Particle Effects for Buttons

Bursting particles effects for buttons. By Luis Manuel.

![Particle Effects](https://tympanus.net/codrops/wp-content/uploads/2018/04/particleeffects_featured.jpg)

[Article on Codrops](https://tympanus.net/codrops/?p=34685)

[Demo](http://tympanus.net/Development/ParticleEffectsButtons/)

## Credits

- [anime.js](http://animejs.com/)

## Basic usage

The `Particles` library depends on [anime.js](http://animejs.com/) to perform animations, so you need to include it before `Particles`.

Then you can start disintegrating/integrating things like:

```html
<!-- Normal HTML element to disintegrate -->
<button class="button">Button</button>

<script src="anime.min.js"></script>
<script src="dist/particles.min.js"></script>
<script>
    // Initialize a new instance of Particles to disintegrate/integrate the button
    var particles = new Particles('.button');

    // Disintegrate the button into particles
    particles.disintegrate();

    // particles.integrate(); // would do the opposite
</script>
```

## Options

For customization, you can pass `options` to `Particles` constructor. That `options` will override the default values, and will be used for any future operation (`disintegrate` or `integrate`). You can also override the `options` for a specific operation. Here is the complete list of `options` available:

| Name                         | Type                    | Default                    | Description |
|------------------------------|-------------------------|----------------------------|-------------|
|`canvasPadding`               | `Integer`               | `150`                      | Padding for the generated `canvas` that will be positioned right behind the target element. A `canvasPadding = 0` will cause the `canvas` and the target element to have the same dimensions. |
|`duration`                    | `Integer`               | `1000`                     | Duration (`ms`) to perform the animations of target element and particles. |
|`easing`                      | `String` or `Function`  | `easeInOutCubic`           | Easing function to perform the animation of target element. It will be passed directly to `anime.js`. |
|`type`                        | `String`                | `circle`                   | Type of particle. Could be any of the following values: `circle`, `rectangle`, `triangle` |
|`style`                       | `String`                | `fill`                     | Style of particle. Could be any of the following values: `fill`, `stroke`. |
|`direction`                   | `String`                | `left`                     | Direction to start disintegrating the element. Could be any of the following values: `left`, `right`, `top`, `bottom`. The opposite `direction` will be used to perform the `integrate` operation. |
|`size`                        | `Float` or `Function`   | Random from `1` to `4`     | Size (`px`) for particles. |
|`speed`                       | `Float` or `Function`   | Random from `-2` to `2`    | Pixels per frame that a particle will be moved. It could be a `function` to set it randomly per particle (as default value). |
|`color`                       | `String`                | Target's `background-color`| Color used to fill the particles. |
|`particlesAmountCoefficient`  | `Float`                 | `3`                        | A coefficient to calculate the amount of particles to animate. A `particlesAmountCoefficient = 0` will result in `0` particles, while bigger values will increase the amount of particles. |
|`oscilationCoefficient`       | `Float`                 | `20`                       | A coefficient to calculate the oscilation of particles while animating. A `oscilationCoefficient = 0` will result in no oscilation (straight movements), while bigger values will increase the oscilation, resulting in a kind of randomness. |
|`begin`                       | `Function`              | `undefined`                | Execute a function at the beginning of the animation. |
|`complete`                    | `Function`              | `undefined`                | Execute a function at the end of the animation. |

## React Version

A React port of the `Particles` library, as well as related documentation can be found in the following repository [react-particle-effect-button](https://github.com/transitive-bullshit/react-particle-effect-button), by Travis Fischer.

## Angular Version

As well as the React port, there is an Angular version of the `Particles` library.
It can be found in the following repository [angular-particle-effect-button](https://github.com/danielpdev/angular-particle-effect-button), by Daniel Popa.

## License

This resource can be used freely if integrated or build upon in personal or commercial projects such as websites, web apps and web templates intended for sale. It is not allowed to take the resource "as-is" and sell it, redistribute, re-publish it, or sell "pluginized" versions of it. Free plugins built using this resource should have a visible mention and link to the original work. Always consider the licenses of all included libraries, scripts and images used.

## Misc

Follow Luis: [Twitter](https://twitter.com/lmgonzalves), [GitHub](https://github.com/lmgonzalves) 

Follow Codrops: [Twitter](http://www.twitter.com/codrops), [Facebook](http://www.facebook.com/codrops), [Google+](https://plus.google.com/101095823814290637419), [GitHub](https://github.com/codrops), [Pinterest](http://www.pinterest.com/codrops/), [Instagram](https://www.instagram.com/codropsss/)

[© Codrops 2018](http://www.codrops.com)
