# Computer Graphics
This repository contains my coursework for CSE306 "Computer Graphics" @ Ecole Polytechnique.

## Ray Tracer
![Sample Render](https://raw.githubusercontent.com/joshuapjacob/computer-graphics/main/Ray%20Tracer/renders/final.png)

### Features
- Spheres
- Reflection
- Refraction (Solid & Hollow)
- Indirect Lighting
- Spherical Lighting (Soft Shadows)
- Basic Parallelization
- Antialiasing
- Triangle Meshes (.obj)
- Bounding Volume Hierarchies Acceleration

### Requirements
- [stb](https://github.com/nothings/stb) (to write image)

### Compilation & Execution
```sh
$ cd Ray\ Tracer/
$ g++ -O3 main.cpp vector.cpp -fopenmp -lpthread -std=c++11 -o main.out
$ ./main.out
```
You can adjust the scene before compiling in ```main()```.

## Sliced Optimal Transport Color Matching
Input | Model | Output
:----:|:-----:|:------:
![](https://raw.githubusercontent.com/joshuapjacob/computer-graphics/main/Color%20Matching/input.png)  |  ![](https://raw.githubusercontent.com/joshuapjacob/computer-graphics/main/Color%20Matching/model.png) | ![](https://raw.githubusercontent.com/joshuapjacob/computer-graphics/main/Color%20Matching/output.png)

### Requirements
- [stb](https://github.com/nothings/stb) (to read/write image)

### Compilation & Execution
```sh
$ cd Color\ Matching/
$ g++ -O3 main.cpp vector.cpp -std=c++11 -o main.out
$ ./main.out input.png model.png 100
```
The last argument is the number of iterations.

## Geometry Processing

- Lab 6:
  - Sutherland-Hodgman Polygon Clipping Algorithm Nanoflann library O(N log N) (section 4.2)
  - Voronoï Parallel Linear Enumeration Algorithm 2D (section 4.3.3 of the lecture notes)

### Compilation & Execution
```sh
$ cd Geometry\ Processing/
$ g++ -O3 main.cpp vector.cpp -fopenmp -lpthread -std=c++11 -o main.out
$ ./main.out
```
