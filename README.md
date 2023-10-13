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
