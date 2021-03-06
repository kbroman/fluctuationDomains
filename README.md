[![DOI](https://zenodo.org/badge/2824581.svg)](https://zenodo.org/badge/latestdoi/2824581)


Fluctuation Domains in Adaptive	Evolution: 
An Example of Reproducible Research in Theoretical Ecology and Evolution

Authors: Carl Boettiger, Johnathan Dushoff, Joshua Weitz
Date: July 12, 2009

This R package is provided as an accompanyment to our paper submitted to Theoretical Population Biology, "Fluctuation Domains in Adaptive Evolution."  Using this pacakge, the reader can directly reproduce the results of this paper, and also explore other parameter regimes and extend the work to other models.  The simulation is written in a fast C code which is compiled into a shared object library that can be utilized by the R functions provided.  

The package structure follows the perscribed format of an R package, with C code in src/ directory, R code in R/ directory, demo scripts in demo.  The current C code relies on the Gnu Scientific Library, developed and maintained by Brian Gough, which is freely available form http://www.gnu.org/software/gsl/ and not included with this package.  This package is provided in the spirit of Reproducible Research in the spirit of Claerbout 1992, following the compedium concept of Gentleman and Temple Lang, 2007.  All the code included in this package is released under the GPL v3 License; included as the file COPYING.  

The current preprint of the paper is found in inst/paper/adpaper.pdf in the source directory, (corresponding to paper/adpaper.pdf in the installed directory).  The package includes functions for reproducing both figures of the manuscript from scratch.  Run demo(adpaper) after loading the library in R to see examples of each of these.  Figure 1, created by the function landscape, is implemented entirely in R and can be used to compute the adaptive landscape and the fluctuation landscape for arbitrary ecological dynamics.  Figure 2 requires the C based simulation, which is controlled from the R function canonical.  Users with a basic knowledge of R should thus be able to reproduce and modify these routines to explore other models.  Users with knowledge of C can easily extend the simulation code to other models by modifying the file logistic.c in the src directory.   The C source code can also be used directly.  


Contact cboettig@ucdavis.edu for support.  


