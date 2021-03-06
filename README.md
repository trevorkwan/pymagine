## Pymagine 

![](https://github.com/katieb1/pymagine/workflows/build/badge.svg) [![codecov](https://codecov.io/gh/katieb1/pymagine/branch/master/graph/badge.svg)](https://codecov.io/gh/katieb1/pymagine) ![Release](https://github.com/katieb1/pymagine/workflows/Release/badge.svg)

[![Documentation Status](https://readthedocs.org/projects/pymagine/badge/?version=latest)](https://pymagine.readthedocs.io/en/latest/?badge=latest)

### Package Overview & Scope

We intend to design functions that provide several different types of visual manipulations to an input image. Note the initial design will accept single images as inputs, but we intend to consider enhancing the package to apply the effects in bulk to a batch of input images.

### Installation:

```
pip install -i https://test.pypi.org/simple/ pymagine
```

### Features

In this package we intend to create four main functions that accept an image as input and apply different types of manipulations and provide a new output image as summarized below:

1. **Barrel 'fisheye' distortion**: produces an image with strong visual distortion intended to create a wide panoramic or hemispherical effect
    - *Stretch goal*: 'pincushion' distortion, effectively the inverse of fisheye distortion
2. **Colour filters**: produces an image with different user-specified colour distortions (ex: sepia tone)
    - *Stretch goal*: allowing the user to specify the strength of the effect via a parameter
3. **Edge detection**: identifies edges by looking at where the image brightness changes sharply, and produces a black and white image highlighting the locations of these edges
    - *Stretch goal*: a more customizable, artistic colourized edge detection filter that would allow the user to specify desired colours for the output image with parameters  (beyond the default black and white) 
4. **Vignetting**: produces an image with reduced brightness around the periphery compared to the image center
    - *Stretch goal*: allow the user to specify a focal point location (other than the centre) via parameter, around which the vignetting effect should be applied

**Package data:** We plan to include a small set of our own photos in the package as sample images for use with the package functions

### Our Package in the Python Ecosystem

A variety of image processing packages providing some similar functionality already exist within the Python ecosystem, including [Pillow](https://github.com/python-pillow/Pillow), [scikit-image](https://github.com/scikit-image/scikit-image), and the more advanced computer vision oriented [OpenCV](https://github.com/opencv/opencv). The purpose of our package is to provide functions that apply some common artistic filter transformations to a given input image.


### Dependencies

- TODO

### Usage

- TODO

### Documentation
The official documentation is hosted on Read the Docs: <https://pymagine.readthedocs.io/en/latest/>

### Credits
This package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
