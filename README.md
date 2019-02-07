TMFinder
========

This is the Temporal Motif Finder in https://github.com/lkovanen/TMFinder, with compling errors fixed.  
Now it is compatible with  the lastest version of lcelib in https://github.com/CxAalto/lcelib/tree/master/containers.



Installation
------------

TMFinder uses [bliss][bliss] to calculate canonical forms of graphs. You need to install bliss separately to use TMFinder:

1. [Download bliss][bliss] (version 0.72 should work) and compile it by
	following the instructions included with it. Make sure to compile the version without GMP, by calling `make` instead of `make gmp`.

2. Add the path of the bliss directory to the environment variables
	`LIBRARY_PATH` and `CPLUS_INCLUDE_PATH`.

You should now be able to compile TMFinder by calling `make` in the directory `src`. If you get an error message about `bliss` or `graph.hh`, recheck your installation of bliss and the environment variables pointing to the location of the bliss library.

After the compiling, make sure everything works by running the test script `tests/test_small.sh`. This should produce a single output file, `test_small_output.dat` that contains information about the temporal motifs in the small test data.

[bliss]: http://www.tcs.hut.fi/Software/bliss/ "bliss"


If you use this code in scientific work, please cite the above publication.

> Lauri Kovanen, Márton Karsai, Kimmo Kaski, János Kertész, Jari
Saramäki, "Temporal motifs in time-dependent networks",
Journal of Statistical Mechanics: Theory and Experiments. P11005 (2011)
doi:10.1088/1742-5468/2011/11/P11005

> Lauri Kovanen, Kimmo Kaski, János Kertész, Jari Saramäki. "Temporal motifs reveal homophily, gender-specific patterns and group talk in mobile communication networks." Proceedings of the National Academy of Sciences, 201307941 (2013). doi:10.1073/pnas.1307941110




