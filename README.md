# lifetime-in-color :framed_picture:
Parsing, interpreting, or visualizing biomedical microscopy data

## Table of contents
1. Fluorescence Lifetime Imageing Microscopy (FLIM) [Image Generator](#flim)
2. Refrences


### FLIM
[Table of contents](#table-of-contents)

Using Becker & Hickl FLIM card and SPCImage software[^1], FLIM curve-fitting models can discern the fluorescence decay patterns in a sample.

![Screenshot of B&H SPCImage Analysis Window](https://github.com/Jack-CC33/lifetime-in-color/blob/main/1.%20FLIM%20Image%20Generator/SPCImage_Screenshot.png)

File>Export allows a user to save color-coded FLIM images, as seen above, but the image generator code in the "FLIM Image Generator" directory lets a user take more control over the image generation and affiliated color scale.

First, export the lifetime data of interest (for the Flipper-TR example, τ₂ is needed) and the intensity image from an image, as below.

![Screenshot of B&H SPCImage Export Window](https://github.com/Jack-CC33/lifetime-in-color/blob/main/1.%20FLIM%20Image%20Generator/SPCImage_Export_Screenshot.png)

### References
[^1]: B&H Handbook.
