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

# Usage
This section provides a few basic examples of how to use the functionality of the project.

## vectAdd.cu
The vectAdd.cu file is used for vector addition. Here is a basic example of how to use it:
// Initialize vectors A and B
float* A = (float*)malloc(size);
float* B = (float*)malloc(size);

// Fill vectors with some values
for(int i = 0; i < N; i++){
    A[i] = i;
    B[i] = i;
}

// Call the function from vectAdd.cu
vectAdd(A, B, N);

## mathAdd.cu
The matAdd.cu file is used for matrix addition. Here is a basic example of how to use it:
// Initialize matrices A and B
float* A = (float*)malloc(size);
float* B = (float*)malloc(size);

// Fill matrices with some values
for(int i = 0; i < N; i++){
    for(int j = 0; j < N; j++){
        A[i*N + j] = i + j;
        B[i*N + j] = i - j;
    }
}

// Call the function from matAdd.cu
matAdd(A, B, N);
