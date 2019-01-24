# Urban Traffic Routing Problem
The code in this repository is an attempt to recreate the algorithm described in the 2013 CEC paper by Mumford [link](https://users.cs.cf.ac.uk/C.L.Mumford/Research%20Topics/UTRP/Outline.html) for solving the urban tranpsort routing problem

The urban traffic routing problem (UTRP) is the problem of designing a set of bus routes that minimize some objectives given a set of bus-stops, the pairwise travel between them, and a matrix estimating total pairwise demand between all bus-stops. Typically one tries to optimize for both the operator (total cost, usually a function of the total length of all bus routes) and the passengers (a function of minimum total transit time and number of changes required).

The UTRP is an NP-hard optimization problem and the approach for tackling it in this implementation is a multi-objective genetic algorithm.

## Running the code
The code in this repository is written in pure C++ 2014 with no libraries or dependencies other than the standard library. To run this code edit the file paths in the preprocessor directives in lines 11 and 12 `main.cpp` to point to a distances matrix and a demand matrix (some sample sample files can be found [here](https://users.cs.cf.ac.uk/C.L.Mumford/Research%20Topics/UTRP/CEC2013Supp.zip). Then compile and run main.cpp

Running 200 iterations on the Mandl test set should take only a few minutes.

