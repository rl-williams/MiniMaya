# MiniMaya

[Cannot upload full code due to academic integrity restrictions.]

## description
Interactive 3D geometry manipulator. A mini version (in essence) of Autodesk's Maya modeling program. Created for Computer Graphics (CIS 277) at the University of Pennsylvania. Created in Qt Creator using C++ and OpenGL.

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

## issues

## credit

Interactive 3D geometry manipulator, 
OBJ loader and exporter, half-edge data structure, Catmull-Clark subdivision, skeletons/joints, and shader-based skin deformation. Also per- sonally implemented raytracing with lambert, phong, reflective, and refractive surfaces and anti-aliasing.
