# DuplicateLearnts
The repository contains the proof-of-concept implementations of duplicate learnts-based heuristic for CDCL SAT solvers and related information. 

The CSV folder contains the rundowns of the computational experiments performed using the provided implementations on the computing cluster "Academician V.M. Matrosov" of Irkutsk Supercomputer Center of the SB RAS. All experiments were launched on computing nodes with the following configuration:
    two 18-core processors Intel Xeon E5-2695 v4 «Broadwell» 2.1 GHz (Base Freq. - Non-AVX), 2.4 GHz (AVX Max All Core Turbo Freq.), 45 MB L3 cache, 128 GB RAM DDR4-2400
with 36 tasks (SAT solver - SAT instance) per node (e.g. each solver always utilized one CPU core with all core loaded). 
The timelimit on SAT solver runtime was set to SAT competition's standard 5000 seconds.


The presented patches can be used to obtain the versions of solvers we employed in our experiments.
The original versions of MapleLCMDistChronoBT and MapleLCMDist can be downloaded from SAT competitions 2018 and 2017, respectively.
The direct download links are presented below:

http://sat2018.forsyte.tuwien.ac.at/solvers/main_and_glucose_hack/MapleLCMDistChronoBT.zip

https://baldur.iti.kit.edu/sat-competition-2017/solvers/main/Maple_LCM_Dist.zip

To patch solvers unzip the sources to a folder, copy patch file to the same folder and run 
patch -p0 < ./<patch_filename>

After this to build each solver it is sufficient to launch ./starexec_build (it might be necessary to chmod +x ./starexec_build first).
