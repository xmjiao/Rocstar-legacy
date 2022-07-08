# Rocstar
Rocstar multiphysics simulation application

Rocstar is a multiphysics simulation application designed to do fluid-structure interaction (FSI) across moving, reacting interfaces. Rocstar couples multiple domain-specific simulation packages and disparately discretized domains and provides several simulation-supporting services including conservative and accurate data transfer, surface propagation, and parallel I/O. Rocstar is MPI parallel and routinely executes large simulations on massively parallel platforms. Rocstar was originally developed at the University of Illinois Center for Simulation of Advanced Rockets (CSAR) under Department of Energy ASCI program funding. Ongoing development of Rocstar is conducted by Illinois Rocstar LLC with company IR&D and continued DOE SBIR funding.

You can access Rocstar Doxygen at: http://illinoisrocstar.github.io/Rocstar/

#Compilation
To compile, make sure that hdf4, hdf5, cgnslib, and metis have been installed,
and then run 

```bash
mkdir build
cd build
FFLAGS=-fallow-argument-mismatch cmake .. 
make -j
```

where FFLAGS=-fallow-argument-mismatch is required for gfortran-11.
For older versions of Fortran, this flag can be ignored.
