# DuplicateLearnts
The repository contains the proof-of-concept implementations of duplicate learnts-based heuristic for CDCL SAT solvers and related information. 

The CSV folder contains the rundowns of the computational experiments performed using the provided implementations on the computing cluster "Academician V.M. Matrosov" of Irkutsk Supercomputer Center of the SB RAS. All experiments were launched on computing nodes with the following configuration:
    two 18-core processors Intel Xeon E5-2695 v4 «Broadwell» 2.1 GHz (Base Freq. - Non-AVX), 2.4 GHz (AVX Max All Core Turbo Freq.), 45 MB L3 cache, 128 GB RAM DDR4-2400
with 36 tasks (SAT solver - SAT instance) per node (e.g. each solver always utilized one CPU core with all core loaded). 
The timelimit on SAT solver runtime was set to SAT competition's standard 5000 seconds.
