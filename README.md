# upc
 A Universal Polygon Calculator for polygonal paper models

These are specific notes for running the upc application, which reads an svg file created by Inkscape containing paths describing a multi-sided polygonal figure.

I. Setting up the environment

    A. Install Python 3

        1. Download it from https://www.python.org/ (not the Windows store)

        2. Launch the executable (defaults are okay, but choose the option to modify the PATH variable).

    B.  Install needed libraries

        1. svgpathtools (ref: https://github.com/mathandy/svgpathtools)

            a. Prerequisites for latest release (13.3 at the time of this writing)

                i.  pip install numpy

                ii. pip install svgwrite

            b. pip install svgpathtools

II. Issues

    A.  Inkscape compatibility

        1.  The application was developed for an upcoming 1.0 version of Inkscape, which is in beta at the time of this writing. Unlike the previous versions, this one places the origin in the upper-left. The application doesn't support a lower-left origin.

        2.  The application doesn't handle grouped paths, so they need to be ungrouped in the input file first.

    B. Running the program
    
        1.  Double click on the file. Since it has a pyw extension, it will not bring up a console window. If you need a console window, change the extension to py.