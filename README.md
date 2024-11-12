# N Queens Problem

## Team Members

- [Grosu Gheorghe](@Gheorghe24) (MPI)
- [Belibova Daniela](@uploveks) (OpenMP)

## Project Description
The goal of this project is to solve the N Queens problem using a serial algorithm, followed by parallelizing it using parallel processing techniques (MPI and OMP). The N Queens problem involves placing N queens on an N×N chessboard such that no two queens threaten each other. The solution will be evaluated on multiple problem sizes, and to identify bottlenecks and optimize performance, the application will be profiled.

## Algorithm Complexity
The serial algorithm used to solve the N Queens problem has an exponential complexity O(N!), as it must check all possible permutations of the queens on the chessboard to find a valid solution. However, by using optimizations (checking the safety of each position), performance can be significantly improved, but the complexity remains exponential.

## Execution Times for Each Problem Size
The algorithm was tested on three datasets corresponding to different N values:

- **Small**: N=12 (Execution Time: 0.013420000 seconds)
- **Medium**: N=15 (Execution Time: 2.687432000  seconds)
- **Big**: N=16 (Execution Time: 18.519619000 seconds)


## Profiling and Bottlenecks

Profiling was conducted using **Intel VTune** to identify major bottlenecks and evaluate each algorithm's performance. 

