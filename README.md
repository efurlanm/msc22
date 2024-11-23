# My MSc

     __  __         __  __ ____
    |  \/  |_   _  |  \/  / ___|  ___
    | |\/| | | | | | |\/| \___ \ / __|
    | |  | | |_| | | |  | |___) | (__
    |_|  |_|\__, | |_|  |_|____/ \___|
            |___/
    My master's degree

*Last edited: 2024-11-23*

This repository contains the implementations made during my master's degree, as well as miscellaneous materials and related information. 

The research project ran from 2019 to 2022 and resulted in three publications and a conference presentation. The theme of the work consists of implementing toy problems applying Python and Fortran resources in a High Performance Computing (HPC) environment, and evaluating the performance results. The material generated can be found at:

- Miranda, E. F. (2022). Common MPI-based HPC Approaches in Python Evaluated for Selected Test Cases. Master’s dissertation, National Institute for Space Research (INPE).
     - Manuscript: <http://urlib.net/ibi/QABCDSTQQW/46C4U9H>
     - Presentation
          - <https://youtu.be/B_xOG9C04xs> (in Portuguese)
          - [Presentation HPC Python [pt-BR] - Miranda 2022.pdf](Presentation HPC Python [pt-BR] - Miranda 2022.pdf)
     - Repository: <https://github.com/efurlanm/msc22/>
- Miranda, E. F., & Stephany, S. (2021). Comparison of High-performance Computing Approaches in the Python Environment for a Five-point Stencil Test Problem. XV Brazilian E-Science Workshop, at XLI Congress of the Brazilian Computer Society (CSBC-2021), 33–40. 
     - Manuscript: DOI [10.5753/bresci.2021.15786](https://doi.org/10.5753/bresci.2021.15786)
     - Online HTML version of the manuscript: <https://efurlanm.github.io/bs21/>
     - Presentation: DOI [10.5281/zenodo.10672455](https://zenodo.org/doi/10.5281/zenodo.10672455) (in Portuguese)
     - Repository: <https://github.com/efurlanm/bs21/>
- Miranda, E. F., & Stephany, S. (2021a). Common HPC Approaches in Python Evaluated for a Scientific Computing Test Case. Revista Cereus, 13(2), 84–98.
     - Manuscript: DOI [10.18605/2175-7275/cereus.v13n2p84-98](https://doi.org/10.18605/2175-7275/cereus.v13n2p84-98)

## Directories

- [stencil](stencil) - the five-point stencil test case, used in a heat transfer problem on a finite surface modeled by the Poison partial differential equation.
- [fft](fft) - the three dimensional fast Fourier transform test case, an algorithm that computes the multidimensional Fourier transform of an 3D array using a fast Fourier transform algorithm.
- [rforest](rforest) - the random forest test case, an ensemble learning method for tasks such as classification and regression.
- [manuscript](manuscript) - master's dissertation sources in LaTeX format.
- [multi-node-gpu](multi-node-gpu) - training a convolutional neural network for the MNIST dataset, using multi-GPU and multi-node data parallelism.

## Useful links

- [SDumont main site](http://sdumont.lncc.br)
- [SDumont user manual from LNCC](http://sdumont.lncc.br/support_manual.php) (in Portuguese)
- [IDeepS project](http://github.com/vsantjr/IDeepS)

## Acknowledgments

Most of the information about SDumont contained in this repository was obtained during INPE's graduate program, and in the project approved by the LNCC with resources from the government of Brazil, without which this work would not be possible.

## License

[Attribution-NonCommercial 4.0 International - CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)
