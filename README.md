# Algebraic Variety Models for High-Rank Matrix Completion

I implemented the algorithm proposed by Ongie et al. on a subset of the Netflix dataset. The data is in the file `ex8_movies.mat` and the code is in the file titled `netflix.m`. I also reimplemented the Mocap dataset analysis from the original paper. To implement this, you also need the Manopt package in matlab. 

----- Original code by Greg Ongie -----
MATLAB code to implement the variety-based matrix completion (VMC) algorithm described in the paper by Ongie et al.:

> G. Ongie, R. Willett, R. Nowak, L. Balzano.
> "Algebraic Variety Models for High-Rank Matrix Completion", in ICML 2017.
> Available online: https://arxiv.org/abs/1703.09631

The main file is `vmc.m`. To get started, see the example scripts:
* `example_uos_sm.m` - Small-scale union-of-subspaces data
* `example_uos_lrg.m` - Large-scale union-of-subspaces data
* `example_hopkins.m` - Small-scale example using Hopkins 155 dataset
* `example_mocap.m`  - Large-scale example using CMU Mocap dataset 

## Version history
* Version 0.1, Updated 7/22/2017

## Author
Greg Ongie ([website](https://gregongie.github.io)) 

## Acknowledgments
Datasets used in the examples are borrowed from:
* Hopkins 155: http://www.vision.jhu.edu/data/hopkins155/
* CMU Mocap: http://mocap.cs.cmu.edu/

Our implementation of randomized svd uses code from:
* Mu Li: [Making Large-Scale Nyström Approximation Possible](https://github.com/mli/nystrom)
* Antoine Liutkus: [Matlab Central](https://www.mathworks.com/matlabcentral/fileexchange/47835-randomized-singular-value-decomposition)

