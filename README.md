# MegaOptim Commandline Interface

The command line interface is part of the smartoptim-python package which contains python API for interaction with the SmartOptim API.

This repository is only for documenting the CLI tool, no code will be pushed here.

## Requirements

* Python 2.7.* / 3+
* [pip](https://pypi.org/project/pip/)

## Installation

```
sudo pip install megaoptim
```

or if using python 3

```
sudo pip3 install megaoptim
```

Note: If you see error `ImportError: No module named PIL`, you need to install `Pillow` as well:

```
sudo pip install pillow
```

## Usage

Available parameters:

* `api-key` - The api key from megaoptim.com
* `dir` - The path of the directory you want to optimize
* `recursive` - Enable or disable recursive scan. Possible values: `1` or `0`. (Default: `0`)
* `outdir` - The path of the directory to savethe optimized photo. Skip to overwrite.
* `compression` - The compression level. Possible values: `intelligent`, `ultra`, `lossless`. (Default: `intelligent`)
* `keep-exif` - Keep or strip the EXIF data. Possible values: `1` or `0`. (Default: `1`)
* `cmyktorgb` - Convert CMYK images to RGB color palette. Possible values: `1` or `0`. (Default: `1`)
* `max-width` - Resize the image to max width. Set 0 to disable. Possible values: (0 or number > 0). (Default: `0`)
* `max-height` - Resize the image to max height. Set 0 to disable. Possible values: (0 or number > 0). (Default: `0`)
* `exclude` - Comma separated list of paths you want to exclude from optimization. Possible values: "/path/to/dir1,/path/to/dir2"

Assuming the megaoptim pip package is installed, the CLI tool can be invoked as follows:

```
megaoptim --api-key=YOURAPIKEY --dir=/path/to/dir --recursive=1 
````
