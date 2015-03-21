**Direct Numerical Simulation of Turbulent Flows**

3dt is a massive-parallel direct numerical simulation code for incompressible turbulent flows in periodic domains based on a spectral method. Additionally, the code can solve for passive scalars with imposed mean shear gradient. The code comprises comprehensive subroutines to calculate flow statistics.

3dt is specially designed to run on JUQUEEN, which is an IBM BG/Q machine. The code employs a two-dimensional domain decomposition strategy based on the excellent library 2DECOMP&FFT. In order to perfectly utilize JUQUEEN a hybrid OpenMP/MPI parallelization approach is implemented. 3dt is currently employed to conduct simulations with 2048<sup>3</sup> and 4096<sup>3</sup> collocation points and reveals linear scaling up to 524k threads which corresponds to 16 mid-planes on BG/Q.

I/O is efficiently implemented by parallel HDF5 or by MPI2-IO.

3dt is written in Fortran 95/2003.

3dt will be released under GPL license soon.
