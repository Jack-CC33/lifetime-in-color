# lifetime-in-color :framed_picture:
Parsing, interpreting, or visualizing biomedical microscopy data

### Table of contents
1. Fluorescence Lifetime Imageing Microscopy (FLIM) [Image Generator](#flim)
2. [References](#references)

---

### FLIM
[Back To Table of contents](#table-of-contents)

Using Becker & Hickl FLIM card and SPCImage software[^1], FLIM curve-fitting models can discern the fluorescence decay patterns in a sample.

![Screenshot of B&H SPCImage Analysis Window](https://github.com/Jack-CC33/lifetime-in-color/blob/main/1.%20FLIM%20Image%20Generator/SPCImage_Screenshot.png)

File>Export allows a user to save color-coded FLIM images, as seen above, but the image generator code in the "FLIM Image Generator" directory lets a user take more control over the image generation and affiliated color scale.

First, export the lifetime data of interest (for the Flipper-TR example, τ₂ is needed) and the intensity image from an image, as below.

![Screenshot of B&H SPCImage Export Window](https://github.com/Jack-CC33/lifetime-in-color/blob/main/1.%20FLIM%20Image%20Generator/SPCImage_Export_Screenshot.png)

Using the ipython notebook file in folder 1, a colormap and bounds can be simply specified to encode the lifetime information.  I suggest using isoluminant colormaps when possible[^2], which lets intensity-encoding lightness remain close to an orthogonal change.  Below are a few examples of the code's use, where a helper function generates a histogram that aids the decision for upper and lower bounds for color-coding the lifetime.

![Example Use of FLIM Image Generator](https://github.com/Jack-CC33/lifetime-in-color/blob/main/1.%20FLIM%20Image%20Generator/Example_Result.png).

### References
[Back To Table of contents](#table-of-contents)
[^1]: B&H Handbook.
[^2]: Colorcet.com; Peter Kovesi. Good Colour Maps: How to Design Them. arXiv:1509.03700 [cs.GR] 2015
