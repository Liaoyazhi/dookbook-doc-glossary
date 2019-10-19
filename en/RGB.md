TOPIC: RGB
AUTHORS: Federico Culloca; federicoculloca@github.com; github:federicoculloca
         Janet Swisher; jmswisher@github.com; github:jmswisher
         Ido Filin; ifilin@mozilla.net; mdn:ifilin

# RGB

Red Green Blue (RGB) is a color model that represents colors as mixtures of three
underlying components (or channels), namely, red, green, and blue. Each color is
described by a sequence of three numbers (typically between 0.0 and 1.0, or between 0 and 255)
that represent the different intensities (or contributions) of red, green, and blue, in
determining the final color.

There are many ways to describe the RGB components of a color. In CSS they can be
represented as a single 24-bit integer in hexadecimal notation
(for example, `#add`8e6 is light blue), or in functional notation as three separate
8-bit integers (for example, rgb(46, 139, 87) is sea green). In OpenGL, WebGL, and GLSL
the red-green-blue components are fractions (floating-point numbers between  0.0  and 1.0),
although in the actual color buffer they are typically stored as 8-bit integers. Graphically,
a color can be represented as a point in a three-dimensional grid or cube, where each dimension
(or axis) corresponds to a different channel.

## Learn More

### General Knowledge

- [RGB color model on Wikipedia](https://en.wikipedia.org/wiki/RGB_color_model)

### Learn About It

- [CSS data type: `<color>`](https://wiki.developer.mozilla.org/en-US/docs/Web/CSS/color_value)
