# libtiny3d – 3D Graphics Engine (Completed Project)

## Project Overview:
libtiny3d is a 4-week systems programming project in which I developed a full-featured 3D graphics engine entirely from scratch in C. The project involved implementing all core components of a software rendering engine without relying on existing graphics libraries like OpenGL or DirectX, providing a deep understanding of the computational and mathematical foundations behind 3D graphics.

### Key Achievements:

Software Rendering Pipeline: Designed and implemented a complete pipeline to convert 3D geometric data into 2D images, including vertex processing, projection, and rasterization.
Custom Math Libraries: Built vector and matrix operations from the ground up to support 3D transformations, rotations, and scaling.
Floating-Point Canvas System: Created a rendering canvas capable of drawing smooth lines and shapes with sub-pixel precision.
Lighting System: Developed lighting algorithms to simulate realistic interactions between light and 3D objects.
Animation Framework: Implemented advanced interpolation techniques to animate 3D objects smoothly over time.
Demonstration: Produced a working demo featuring animated, lit 3D wireframe objects, showcasing the engine’s capabilities.

### Outcome:
The project provided hands-on experience with low-level systems programming, linear algebra, and real-time rendering concepts. It successfully demonstrated the ability to construct a functioning 3D graphics engine from first principles, highlighting both technical depth and software design skills.

## 3d-renderer-library

This library defines some functionalities and improvisations that can be implemented related to 3d rendering and drawing in a canvas in C language related build enviornments.

Use the files in this library as needed

### Key features

#### canvas.h
-for 2D line drawing with improvised smoothness
-to save a drawn canvas as a ppm file to be used as needed

#### math3d.h
-describes key mathematical functions related to smooth and precise 3D rendering and projections

#### renderer
-render 3d wireframes and implement rotations and translations on them
-output your transformations framewise
-depth sorting according to camera view and realistic projections
-brightness changes according to edge distance with the viewer

#### lightsource_renderer.h
-render the objects with effect of multiple implemented light sources

#### lightning.h
-determine the brightness of lines according to present conditions in the virtual enviornment

### Demonstrations
-Line smoothness depicting
-Depth sorted and brightness corrected 3D wireframes
-Effect of light sources on objects

To use the 3D Rendering Library, you may need to convert **PPM (Portable Pixel Map)** files into more widely-used image formats such as **JPEG** or **GIF**. The **ImageMagick** tool provides a simple way to do this.

#### Prerequisites
Install **ImageMagick** on your system if you haven't already. ImageMagick is a powerful image manipulation tool that includes the `convert` command, which is used for file format conversion.

#### How to run

Run this file and demonstartions in linux or simmilar enviornment
To create the demonstartions in a terminal opened in the root directory write thefollowing commands

###### To get the clock_line demonstration
make clock_lines

###### To get the clock_line demonstration
*$ make clock_lines*

###### To get the soccer ball demonstration
*$ make soccerball*

This may take a while to get executed fully

###### To get the light source implemented demonstration
*$ make light_source*

This may take a while to get executed fully

You can also run all the three executions subsequently by 
*$ make all* or *$ make*

### Other
Special function related to finding the vertices pairs to be matched when drawing a truncated icosahedron is included
Also some example renderings done using this had been attached in the **visual_tests**
