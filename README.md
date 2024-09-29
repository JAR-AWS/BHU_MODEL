To run the simulations, you will first need to download and install Castro by following the instructions on https://amrex-astro.github.io/Castro/docs/getting_started.html

Don't forget to add the home directory to your path using the following command.

export CASTRO_HOME="/path/to/Castro/"

Note: You must export the path to "CASTRO_HOME" and not a different name unless you want to modify the name in the makefile.

Once you have completed the above steps, download and extract the specific simulation directory that you want to run from this repository.

Steps to run:
1. Open the downloaded problem directory.
2. Open the terminal inside the directory and type "make" in the command line. (without the quotations)
3. Now, the code will start to compile.
4. Once the compilation is done, run the following command to start the simulation:
   
   mpirun -np n ./Castro1d.gnu.MPI.ex inputs_1d
   
   (replace "n" with the number of processors you want to use)
   
6. Wait till the simulation ends.

Castro outputs in boxlib format, which is not easy to read with the usual tools (especially the 1D datasets cannot be plotted with AmrVis, visit, ParaView
and other plotting tools). 
So, we use a tool called yt to read the files and plot the data. We have provided a Jupyter notebook that you can use to visualize the data using yt. 
You will first need to install yt in your Python environment. Refer to the following guide for installation:
https://yt-project.org/doc/installing.html

Now, you are all set to run cool simulations of the cold collapse of massive, spherically symmetric and homogenous cold clouds (Newtonian) and compare the results with the GR version of the same.
