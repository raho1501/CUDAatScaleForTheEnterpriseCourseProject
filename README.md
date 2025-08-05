# Sobel-filter on image using NVIDIA NPP with CUDA

## Overview

This project demonstrates the use of NVIDIA Performance Primitives (NPP) library with CUDA to perform a sobel filter on an input image. 
The goal is to utilize GPU acceleration to efficiently execute the filter kernel on a given image, leveraging the computational power of modern GPUs. 
The project is a project submission for the cource CUDA at Scale for the Enterprise.

## Code Organization

```bin/```
This folder containes the built executable after the build is successful.

```data/```
This folder contains the input-data for the program as well as the result of after the program. The output is prefixed with ```sobel_```.

```src/```
The source is in this folder.

```README.md```
This file should hold the description of the project so that anyone cloning or deciding if they want to clone this repository can understand its purpose to help with their decision.

```INSTALL```
To run this code. Clone the repo into the laboratory environment into the ```project``` folder. The environment contains all required dependecies.

```Makefile```
Use the makefile to build and manage the code.
-  ```make``` Build the project.
- ```make run```  Runs the project with default parameters
- ```make clean``` Clean up the build files.
- ```make help``` Display the help message.

## Running the Program
After building the project, you can run the program using the following command:

```bash
Copy code
make
make run
```

This command will execute the compiled binary, performing the sobel-filter on the input image (sloth.pgm), and save the result as sloth_sobel.pgm in the data/ directory.

If you wish to run the binary directly with custom input/output files, you can use:

```bash
- Copy code
./bin/imageSobelNPP --input data/sloth.pgm --output data/sloth_sobel.pgm
```

- Cleaning Up
To clean up the compiled binaries and other generated files, run:


```bash
- Copy code
make clean
```

This will remove all files in the bin/ directory.
