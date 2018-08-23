# Parallel-Strtegies-for-K-means-algorithm


The project implements four versions code of K-means algorithm, three parallel programs (MPI, OpenMP and Hybrid MPI&OpenMP)


Before Run:

The parallel codes employ MPI and OpenMP library, which requires to intall manually. We select Intel compiler to compile our codes.

Enter: "module load intel-compilers-17" and "module load intel-mpi-17"


Compile:

Run: make

For each version, there is a "Makefile" file which contains the compiling directives. User only need to enter "make", then the code will be compiled automatically and executable of k-means algorithm will be created.


Submit to backend nodes:

Run: qsub run.pbs


The job script in each version is named by "runXXX.pbs", users enter the command"qsub runXXX.pbs" could submit jobs to the backend nodes. The result is written into a txt file named by "resultXXX.txt" anda text file called "label_result.txt" is created which shows the memership of points.
