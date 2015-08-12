# MiniMaya

[Cannot upload full code due to academic integrity restrictions.]

## description
Interactive 3D geometry manipulator created in Qt Creator using C++ and OpenGL. A mini version (in essence) of Autodesk's Maya modeling program. Created for Computer Graphics (CIS 277) at the University of Pennsylvania.

Project completed individually over the course of two months. Added final features (freeform deformation lattice, keyframe animation, raytraced scene output) as a group of three, in which I was personally responsible for the latter feature.

## features
- OBJ Loader and Exporter
  - program automatically loads a unit cube mesh, but the user may use the GUI to import any regularly-formatted .obj file and create a mesh with half-edge structure
  - manipulate geometry and then export the new vertex data to a new .obj file
- Geometry Selection
  - Pick elements of geometry (either from the auto-loaded unit cube or from an imported mesh) using the mouse pointer on the view screen or from an auto-filled list of vertices, edges, and faces
  - When an edge is selected, use the GUI to select either its next or symmetric edge
  - Selection is visible both on-screen with a color change and in the lists of relevant elements
- Geometry Manipulation
  - translate vertices using XYZ sliders
  - split an edge evenly into two edges (and its symmetric edge into two as well) using the "add" button while an edge is selected
  - change face color using RGB sliders
  - split a quadratic face evenly/diagonally into two triangles using the "triangulate" button while a face is selected
  - smooth mesh via Catmull-Clark subdivision techniques using the "smooth" button (cube converges to a spherical shape when smoothed multiple times)
- Joint and Skin Deformation
  - load a JSON file that describes a skeleton joint heirarchy and attributes; joints become visible on screen and may be transformed using translation and rotation buttons
  - select the "skin" button while a joint of the skeleton is selected (from the auto-produced list of elements) to give joints influence over vertices (amount of influence is determined by proximity).
  - once a mesh has been "skinned," the user may again select and manipulate joints; this time, vertices are transformed based on the joints that influence them via a shader-based skin deformation.










- Raytracing
- Animation (implemented by group member)
- Deformation (implemented by group member)

Interactive 3D geometry manipulator, 
OBJ loader and exporter, half-edge data structure, Catmull-Clark subdivision, skeletons/joints, and shader-based skin deformation. Also pesonally implemented raytracing with lambert, phong, reflective, and refractive surfaces and anti-aliasing.
