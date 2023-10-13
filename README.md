# MPI Setup Guide for Ubuntu

This guide will walk you through setting up MPI (Message Passing Interface) on Ubuntu. MPI is a popular framework for writing parallel and distributed applications, often used in high-performance computing.

## Prerequisites

1. **Ubuntu**: This guide is written for Ubuntu, so you should have an Ubuntu machine or VM.

2. **Terminal**: You will need a terminal for running commands.

## Steps

### Step 1: Install MPI

OpenMPI is a popular MPI implementation for Ubuntu. You can install it using apt.

```bash
sudo apt-get update
sudo apt-get install libopenmpi-dev


Simple MPI code



#include <mpi.h>

int main(int argc, char **argv) {
  MPI_Init(&argc, &argv);

  int my_rank;
  MPI_Comm_rank(MPI_COMM_WORLD, &my_rank);

  printf("Hello from rank %d!\n", my_rank);

  MPI_Finalize();

  return 0;
}

To compile this program, you can use the following command:


mpicc hello_world.c -o hello_world 


To run the program on 4 processors, you can use the following command:

mpirun -np 4 hello_world


