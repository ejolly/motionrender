# Motion Render

A motion tracking 3D movie renderer in Python 3.

This package creates movies from motion capture data.  For example, this project
was developed to render movies for research projects using a simple
Kinet 3D skeletion tracking position estimator.  Data is expected to be
in a simple csv format, consisting of a timestamp and then 3D position of
a set of joints. 

The package provides functions to load in data, help convert it to
the needed format, and render the data as images and movies.  The
package relies on Python 3 Matplotlib plotting and movie animations
using the and `matplotlib.animation`
libraries.  This package uses mpeg as a back end renderer to create
the rendered animations.


## Development

Install `ffmpeg` using your system package manager, e.g.
`sudo apt install ffmpeg` on Ubuntu  
`brew install ffmpeg` on MacOS (with [homebrew](https://brew.sh/))


1. `git clone https://github.com/DerekHarter/motionrender`
2. `cd motionrender`
3. `pip install -r requirements-dev.txt`
4. `pip install -e .` Install in dev mode so changes are automatically updated
5. `pytest` to run all tests or `pytest -k testname ` to run a specific test
