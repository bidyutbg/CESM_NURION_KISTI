# CESM_NURION_KISTI
Compilation scripts for CESM on Nurion (Kisti)

Nurion supercomputer is managed and maintained by the Korea Institute of Science and Technology Information (KISTI) National Supercomputing Center, Korea. Nurion's compute nodes are 8,305 Intel Xeon Phi processors (named "Knight Landing") nodes and CPU-only nodes are 132 Intel Xeon processors (named "Skylake") nodes. 

Here are the config_batch.xml, config_compilers.xml and config_machines.xml scripts used to compile the CESM2.1.3 model in the Nurion (KISTI) for both type of processors, namely, MACH="kisti-knl" and MACH="kisti-skl.

I build the model on "kisti-skl" processors using the command:

./create_newcase --case CTRL --machine kisti-skl --compiler intel --compset FHIST --res f09_f09_mg17  # for norm_skl queue)

But one can use the following as well:

./create_newcase --case CTRL --machine kisti-knl --compiler intel --compset FHIST --res f09_f09_mg17  # for normal/long queue)


