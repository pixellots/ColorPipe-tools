Plot that LUT
========================

Plot that LUT is a python script for plotting look up tables.
It uses [OpenColorIO](http://opencolorio.org/) to read input LUTs and [matplotlib](http://matplotlib.org/) to plot results.

Supported LUT formats : 3dl, ccc, cc, csp, cub, cube, hdl, look, mga/m3d, spid1d, spi3d, spimtx, vf.
See [OpenColorIO FAQ](http://opencolorio.org/FAQ.html) for more informations.

Requirements
------------
- Python
- matplotlib + a backend (for exemple Qt, Gtk...)
- OpenColorIO binding

Tested config
-------------
- Python 2.6, Qt 4.8, OpenColorIO 1.0.8, matplotlib 1.2 on openSuse 12.1

Usage
-----
To plot a 1D LUT : ./plotThatLut.py < path to a lut > 1D < samples count >
>plotThatLut.py testFiles/identity.csp 1D 256

To plot a 3D LUT : ./plotThatLut.py < path to a lut > 3D < cube size >
>plotThatLut.py testFiles/identity.3dl 3D 17

Screenshots
-----------
![identity 3D](https://dl.dropboxusercontent.com/u/2979643/identity_3D_LUT.png "identity 3D")

![Rec709 1D](https://dl.dropboxusercontent.com/u/2979643/Rec709_1D_LUT.png "Rec709 1D")