# MendelKinship

This [Julia](http://julialang.org/) package computes genetic kinship and other identity coefficients. MendelKinship is one component of the umbrella [OpenMendel](https://openmendel.github.io) project.

[![](https://img.shields.io/badge/docs-current-blue.svg)](https://OpenMendel.github.io/MendelKinship.jl)

## Installation

*Note: The three OpenMendel packages (1) [SnpArrays](https://openmendel.github.io/SnpArrays.jl/latest/), (2) [MendelSearch](https://openmendel.github.io/MendelSearch.jl), and (3) [MendelBase](https://openmendel.github.io/MendelBase.jl) must be installed before any other OpenMendel package will run. It is easiest if these three packages are installed in the above order and before any other OpenMendel package.*

Within Julia, to install MendelKinship use the package manager (invoked via the `]` key, and escaped via the backspace key) and type:

    pkg> add https://github.com/OpenMendel/MendelKinship.jl

This package supports Julia v1.0+

## Tutorial

A tutorial for MendelKinship is available at [kinship-tutorial](https://github.com/OpenMendel/Tutorials/blob/master/Kinship/KinshipTutorial.ipynb) from the OpenMendel Tutorials github page. 

## Data Files

To run this analysis package you will need to prepare a Control file and have your data files available. The Control file holds the names of your data files and any optional parameters for the analysis. Details on the general format and contents of the Control and data files can be found on the MendelBase [documentation page](https://openmendel.github.io/MendelBase.jl). Descriptions of the specific options available within the MendelKinship analysis package are in its [documentation page](https://openmendel.github.io/MendelKinship.jl).

There are example data files in the "data" subfolder of each Mendel package.

## Running the Analysis

To run this analysis package, first launch Julia. Then load the package with the command:

     julia> using MendelKinship

Next, if necessary, change to the directory containing your files, for example,

     julia> cd("~/path/to/data/files/")

Finally, to run the analysis using the parameters in the control file Control_file.txt use the command:

     julia> Kinship("Control_file.txt")

*Note: The package is called* MendelKinship *but the analysis function is called simply* Kinship.

## Citation

If you use this analysis package in your research, please cite the following reference in the resulting publications:

OPENMENDEL: a cooperative programming project for statistical genetics. Zhou H, Sinsheimer JS, Bates DM, Chu BB, German CA, Ji SS, Keys KL, Kim J, Ko S, Mosher GD, Papp JC, Sobel EM, Zhai J, Zhou JJ, Lange K. *Human Genetics* (2019). DOI: 10.1007/s00439-019-02001-z

<!--- ## Contributing
We welcome contributions to this Open Source project. To contribute, follow this procedure ... --->

## Acknowledgments

This project is supported by the National Institutes of Health under NIGMS awards R01GM053275 and R25GM103774 and NHGRI award R01HG006139.
