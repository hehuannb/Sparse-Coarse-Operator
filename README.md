# sparse-coarse-operator

## Authors:[Ru Huang](https://www.linkedin.com/in/rh1994), Kai Chang, [Huan He](https://hehuannb.github.io/), [RuiPeng Li](https://people.llnl.gov/li50),[Yuanzhe Xi](http://www.math.emory.edu/~yxi26/)

This work was performed under the auspices of the U.S. Department of Energy by Lawrence Livermore National Laboratory under Contract DE-
AC52-07NA27344 and was supported by the LLNL-LDRD program under Project No. 23-FS-031

## Overview 
We propose a data-driven and machine-learning-based approach to compute 
non-Galerkin coarse-grid operators in algebraic multigrid (AMG) 
methods, addressing the well-known issue of increasing operator 
complexity. Guided by the AMG theory on spectrally equivalent 
coarse-grid operators, we have developed novel ML algorithms that 
utilize neural networks (NNs) combined with smooth test vectors from 
multigrid eigenvalue problems. The proposed method demonstrates promise 
in reducing the complexity of coarse-grid operators while maintaining 
overall AMG convergence for solving parametric partial differential 
equation (PDE) problems. Numerical experiments on 
anisotropic rotated Laplacian and linear elasticity problems 
are provided to showcase the performance and compare with existing methods for  computing non-Galerkin coarse-grid operators.

### Example
Please check out the [jupyter notebook](tests/laplacian/fixed-xi/laplacian-test-xi10.ipynb).

### Model
Our main model architecture can be found [here](libs/models.py). The freuqency encoder is defined in  


### Lisence
THe codebase is under MIT license. For individual dataset usage, please refer to the dataset license found in the website.