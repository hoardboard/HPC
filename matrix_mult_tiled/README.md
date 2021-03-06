### Matrix multiplication

Basic parallel matrix multiplication using CUDA.
This implementation differs from [the previous one](http://github.com/pin3da/HPC/tree/master/matrix_mult)
in the allocation of the memory on the GPU. In this case we attempt to
use the shared memory of the device.

Directories description:
- src : Matrix multiplication code
- test : Matrix generator

A simple plotter is also provided, you can make uggly graphics like this

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult/matrix_mul.png)

### Compile and running

create a build directory

    mkdir build
    cd build

create cmake stuff

    cmake ..

compile & run

    make
    generator > input
    mult < input > data

### Performance graphics


![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/figure_1.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/figure_2.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/figure_3.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/tiling1.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/tiling2.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/4_8.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/8_16.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/16_32.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/float8.png)

![Matrix image](https://raw.githubusercontent.com/pin3da/HPC/master/matrix_mult_tiled/images/float4_8.png)

