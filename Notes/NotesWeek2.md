# [3D Graphics - Basic Concepts](https://canvas.berklee.edu/courses/27773/pages/3d-graphics-basic-concepts?module_item_id=1485479)
### Graphics Pipeline
shader: application(CPU) -> geometry processing(GPU) -> rasterization(CPU) -> pixel processing(GPU)     
stages are dependent on the result of the result of the previous stage, and if a stage slower than the others it becomes a bottleneck and determines the speed of the process.

#### Ray tracing basics
* A ray is cast for each pixel
* Z-Buffer

#### Camera
* the view frustum
    * a virtual camer rendering a scene with perspective can be thought of as being located at the tip of a pyramid
    * Inside the pyramid, there is a view volume, namely the frustum, i.e. a truncated pyramid with a rectangular base. only the inside of the frustum will be rendered
    * Frustum is denoted by a near plane and a far plane
* Camera Modes
  * Perspective
    * elements get smaller the farther they are from the camera
    * usually used in 3D games
  * Orthogonal
    * Everything is shown as flat, no perspective
    * Mostly used in 2D or Birds Eye View games (LoL was used as an example)

#### Scene Graph
* Trees
  * Parent/Child Relationships
    * Root Node
    * Leaf Node (node with no children)


The backs of objects are never rendered (if you see the back of a characters head, their face is not rendered)