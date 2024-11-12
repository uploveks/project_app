# Fractal Image Generator - Mandelbrot and Julia

## Team Members

- [Grosu Gheorghe](@Gheorghe24) (MPI)
- [Belibova Daniela](@uploveks) (OpenMP)

## Project Description
This project implements the algorithms for generating Mandelbrot and Julia fractals using serial versions, followed by parallelized versions. Fractals are complex images created based on mathematical formulas, with each pixel representing points in a complex plane. The project's goal is to optimize performance by converting serial algorithms into parallel versions using OpenMP and MPI, reducing execution time for large images and exploring the benefits of parallelization.

## Mandelbrot and Julia Algorithms

### Mandelbrot Algorithm
The Mandelbrot algorithm uses the formula: 
- **z = z^2 + c**,  
where `z` and `c` are complex numbers, with `c` representing the complex plane coordinates corresponding to each pixel in the image. The algorithm iterates the formula until `|z| > 2` or the maximum iteration count is reached. The number of iterations determines the color of each pixel.

### Julia Algorithm
The Julia fractal uses a similar formula: 
- **z = z^2 + k**,  
where `k` is a fixed


## Algorithm Complexity
Both algorithms have a complexity of **O(W × H × I)**, where:
- **W** and **H** are the image dimensions (number of pixels horizontally and vertically),
- **I** is the maximum number of iterations set for each point in the complex plane.


## Profiling and Bottlenecks

Profiling was conducted using **Intel VTune** and **AMD MProf** to identify major bottlenecks and evaluate each algorithm's performance. 

