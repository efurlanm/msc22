#  My thesis

## Abstract

A number of the most common MPI-based high-performance computing approaches available in the Python programming environment of the LNCC Santos Dumont supercomputer are compared using three selected test cases. Python includes specific libraries, development tools, implementations, documentation and optimization or parallelization resources. It provides a straightforward way to allow programs to be written with a high level of abstraction, but the parallelization features to exploit multiple cores, processors or accelerators such as GPUs are diverse and may not be easily selectable by the programmer. This work compares common approaches in Python to increase computing performance for three test cases: a 2D heat transfer problem solved by the finite difference method, a 3D fast Fourier transform applied to synthetic data, and asteroid classification using a random forest. The corresponding serial and parallel implementations in Fortran 90 were taken as references to compare the computational performance. In addition to the performance results, a discussion of the trade-off between easiness of programming and computational performance is included. This work is intended as a primer for using parallel HPC resources in Python.

## Implementations

| Directory | Description                                                                                                                                                                        |
|:---------:| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| stencil   | The five-point stencil test case, used in a heat transfer problem on a finite surface modeled by the Poison partial differential equation.                                         |
| fft       | The three dimensional fast Fourier transform test case, an algorithm that computes the multidimensional Fourier transform of an 3D array using a fast Fourier transform algorithm. |
| rforest   | The random forest test case, an ensemble learning method for tasks such as classification and regression.                                                                          |
| thesis    | My original master's thesis in LaTeX format.                                                                                                                                       |

## Note

<table>
    <tr>
        <td><img src="img/construction.gif"></td>
        <td>This repository is permanently under construction, so its content changes constantly</td>
    </tr>
</table>
