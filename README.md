# SorghumReconstructionAndPhenotyping
Program to reconstruct sorghum plants from depth images and make measurements of the reconstruction

This software is provided as is, without warranty or guarantee that it will work, and many features remain untested.

# Contact
Ryan McCormick

# Dependencies
- RapidXML - http://rapidxml.sourceforge.net/
- OpenCV - http://opencv.org/
- PCL - http://pointclouds.org/
  - (and the PCL's dependencies; e.g. Boost, Eigen, VTK)

# Compilation
First, make sure you can compile a project that depends on PCL and OpenCV (e.g., http://codextechnicanum.blogspot.com/2014/10/installing-point-cloud-library-and.html). On an Ubuntu system, PCL and OpenCV can be obtained from the apt package manager, but I recommend compiling PCL from source (e.g., http://pointclouds.org/documentation/tutorials/compiling_pcl_posix.php) so that you have access to an up to date version and ability to turn on things like fitting NURBS and B-splines (e.g., http://pointclouds.org/documentation/tutorials/bspline_fitting.php).

If you can compile PCL and code that depends on PCL, you should be able to use those build options in your IDE of choice, add all of the source files to your project, and compile. At some point in the future, an improved installation process will hopefully be added.

As a personal note, the hardest part (for me) was tracking down where on your system the necessary libraries are stored. You can find a list of the necessary includes and libs to link to in the MAKEFILE. The MAKEFILE itself was autogenerated from a CodeBlocks configuration and is untested, and is provided more as an example of the includes and libs you need rather than something that you can expect to run make with.
