cmake_minimum_required(VERSION 3.15)
project(MPI_Examples C)

set(CMAKE_C_STANDARD 99)

add_executable(MPI_Examples main.c)
set(CMAKE_C_COMPILER mpicc)
set(CMAKE_CXX_COMPILER mpicxx)
target_link_libraries(MPI_Examples mpi)