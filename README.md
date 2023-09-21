This repository contains a collection of CUDA programs that perform various mathematical operations on matrices and vectors. 
These operations include matrix multiplication, matrix scaling, softmax function implementation, vector addition, matrix addition, and dot product calculation. 
The programs are designed to leverage the parallel processing capabilities of GPUs to perform these operations more efficiently than traditional CPU-based implementations.

The programs are written in C and use CUDA for GPU programming. They define kernel functions that perform the operations on the GPU, and main functions that handle memory allocation, data initialization, data transfer between the host and device, kernel launching, result printing, and memory cleanup. The programs also include necessary header files and use random data for testing.
# Prerequisites
Before you start, ensure that you have the following:

-A C compiler that supports the standard library headers <stdio.h> and <stdlib.h>.
-The CUDA toolkit, which includes the CUDA runtime library and the necessary headers for GPU programming.
-A compatible GPU device with CUDA support.
-Sufficient memory allocation for the host and device arrays used in the program.