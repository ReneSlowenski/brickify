# Brickfy [![Build Status](https://travis-ci.org/JuanPotato/Brickfy.svg?branch=master)](https://travis-ci.org/JuanPotato/Brickfy) [![PyPI Downloads](https://img.shields.io/pypi/dm/brickfy.svg)](https://pypi.python.org/pypi/brickfy) [![PyPI version](https://img.shields.io/pypi/v/brickfy.svg)](https://pypi.python.org/pypi/brickfy) [![License](https://img.shields.io/pypi/l/brickfy.svg)](https://pypi.python.org/pypi/brickfy) [![Coverage Status](https://coveralls.io/repos/JuanPotato/Brickfy/badge.svg?branch=master&service=github)](https://coveralls.io/github/JuanPotato/Brickfy?branch=master) [![Code Health](https://landscape.io/github/JuanPotato/Brickfy/master/landscape.svg?style=flat)](https://landscape.io/github/JuanPotato/Brickfy/master) [![Join the chat at https://gitter.im/JuanPotato/Brickfy](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/JuanPotato/Brickfy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)


### What is it?
Brickfy is a python program that takes a static image or gif and makes it so that it looks as if it was built out of interlocking bricks.

<a href="https://commons.wikimedia.org/wiki/File:Zoysia_grass_flower.jpg">
<img alt="Before" title="Before (The inflorescence of Zoysia grass, a variety of lawn grass. Picture by Hari Krishnan)" height="500" src="brickfy/assets/flower.jpg?raw=true">
</a>
<img alt="After" title="After" height="500" src="brickfy/assets/flower_brick.png?raw=true">


### Requirements
* Python
* Python modules: Pillow, click # pip will install these automatically if using `pip install brickfy`
* imagemagick # not needed but recommended

### Bugs
If you find a bug:
  1. Check in the [open issues](https://github.com/JuanPotato/Brickfy/issues) if the bug already exists.
  2. If the bug is not there, create a [new issue](https://github.com/JuanPotato/Brickfy/issues/new) with clear steps on how to reproduce it.

### Quickstart
install from source
```shell
$ git clone https://github.com/JuanPotato/Brickfy.git
$ cd Brickfy
$ python setup.py install
```

### Usage
```
Usage: brickfy [OPTIONS] IMAGE [OUTPUT]

  Brickfy an image!

Options:
  --size INTEGER                  Number of bricks the longest side of the brickfied image should have.
  --dither / --no-dither          Use dither algorithm to spread the color approximation error.
  --palette [all|effects|mono|solid|transparent]
                                  Palette to use based on real Brick colors.
  --help                          Show this message and exit.
```

#### Palette
There are 3 palettes: solid (33 colors), transparent (14 colors) and effects (4 colors).
You can use one of them or all the 3.
```shell
$ brickfy --palette solid image.jpg
$ brickfy --palette transparent image.jpg
$ brickfy --palette effects image.jpg
$ brickfy --palette all image.jpg
```
There is another one palette, mono, with only 2 colors (black and white...). It's just for test and fun...

### Installation
1. Download and install all requirements
 * python from the [official python website](https://www.python.org/)
 * imagemagick from the [official imagemagick website](https://imagemagick.org/)
2. Download this project by using the download zip button on this page, or running `git clone https://github.com/JuanPotato/Brickfy`
 * If you downloaded a zip file, please unzip it
3. Open a command line and navigate to the project folder
4. Run `python setup.py install` while in the project folder
5. You can now use Brickfy anywhere, see [usage](#usage) for more help

