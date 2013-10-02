** Photometric stereo using light from monitor (e.g., laptop, desktop) **
** Tony TUNG (c) 2011-2013

The current implementation is a beta version I developed for testing.
It is distributed for fun and education.

It works with the following set of images: pic.tar.gz (available at tonytung dot org)
Please, respect the privacy of the authors and do not re-distribute the materials.
A similar setup relying on photometric stereo using SVD was presented in [Schindler, 3DPVT08].

You can easily make you own set of input images using your own computer screen.
Create 5-6 presentation slides (e.g., using PowerPoint) containing one white rectangle on black background. 
The rectangles will serve as light sources and should be placed on each side and a the center, in each slide respectively.
Capture your face with a webcam while displaying each slide one by one.
Don't move! (Put a timer on your slides and capture software!)

Source code written in C++. It requires OpenCV2.x libraries to work.

Place the images in the same folder as the binary file
Run the program like this: ./photostereo 4
It will load 4 images. Try with different numbers (3,5,6..).
Among the several outputs, you may find a pointcloud: poincloud.off. You can view it with MeshLab or Geomview.
With the given set of images, the result should be as shown below (3D point clouds and input images).
Geometry in central regions (eyes, nose, mouth) and details on T-shirt is OK. Not perfect at borders.
