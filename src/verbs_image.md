# Image/sprite verbs
---

`(doubleres)`: Causes Etterna to halve the size of the image that has
        this verb applied.
- Useful for: Packing detail into subpixels, if you're into that kind of thing.

`(res wxh)`: Causes Etterna to scale the image that has this verb applied to the
        specified resolution.
        Replace "wxh" with the actual x of the image.
- Useful for: Fixing scaling bugs that may occur when using images that aren't
        scaled to a power of 2.

`(dither)`: Undocumented verb, likely has something to do with applying
        color dithering to the image.
- Useful for: N/A

`(stretch)`: Allows some types of images to be used with `texcoordvelocity`
        and `customtexturerect` without graphical glitches.
- Useful for: Themes that use potentially unsafe actor commands with images.

`(mipmaps)`: Undocumented verb, likely applies ["mipmaps"](https://en.wikipedia.org/wiki/Mipmap) to an image.
- Useful for: N/A

`(nomipmaps)`: Undocumented verb, likely the opposite of `(mipmaps)`.
- Useful for: N/A

`(grayscale)`: Converts an image from full-color to grayscale.
        An interesting thing of note is that images without alpha get
        converted to 8-bit grayscale, while images with alpha get 7-bit.
- Useful for: N/A

`(alphamap)`: Indicates that the only component in the texture is the alpha
        channel, discards all color.
- Useful for: Applying alpha masks to images; only use if you fully understand
        the verb, and what it does.

`(32bpp)`: Sets the color depth of the image to 32 bits per pixel.
- Useful for: N/A

`(16bpp)`: Sets the color depth of the image to 16 bits per pixel.
- Useful for: N/A

