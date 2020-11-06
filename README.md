# CppAlgo
This is a repository that specialize in C++ algorithms with lower level accelerations. It mainly 
relies on the Intel ecosystem and CUDA eco-system. 

To use the examples, it is required to install 

1. [Intel Parallel Studio](https://software.intel.com/content/www/us/en/develop/tools/parallel-studio-xe.html).
2. [cmake](https://cmake.org/).
3. [boost](https://www.boost.org/).
4. [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads).
5. [GTest](https://github.com/google/googletest).

All the examples are built in Linux. We will also be using C++ 14 (mainly to use Hana).

## Compilation
Since we will be using icc as compiler, the correct way to compile
the programs is

`cmake .. -DCMAKE_C_COMPILER=icc -DCMAKE_CXX_COMPILER=icpc -DCMAKE_Fortran_COMPILER=ifort`

## Suggestions
1. Use [gdbgui](https://www.gdbgui.com/) is a great way to find bugs.
2. Use Intel Vtune to identify hotspots. 