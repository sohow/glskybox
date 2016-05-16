# glskybox

A simple python tool for converting skysphere texture to skybox.

## Requirements

* [PyOpenGL](http://pyopengl.sourceforge.net/) The Python OpenGL Binding
* [Pillow](https://pypi.python.org/pypi/Pillow) Python Imaging Library

`pip install -r requirements.pip`

## Usage

    usage: glskybox.py [-h] [-o OUTPUT] [-s SIZE] [-f] FILE [FILE ...]
    
    Convert skydome texture to skybox
    
    positional arguments:
      FILE                  source file name(宽高像素值必须是2的n次方)
    
    optional arguments:
      -h, --help            show this help message and exit
      -o OUTPUT, --output OUTPUT
                            destination path
      -s SIZE, --size SIZE  output image size
      -f, --overwrite       overwrite existing output

Example:

Use a photo taken by [PhotoSphere](https://www.google.com/maps/streetview/publish/) app, then run:

`python glskybox.py your_sphere_photo.jpg`

Check out the result in output/ directory.

If you give a directory as input, it will traverse all files inside it and render them.
