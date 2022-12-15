# New Keynesian Model using Python and Dynare++

This repository shows an example of how to use Dynare++ from Python. For this, a New Keynesian Model (Galí Ch.3) is solved. The entire model and .mod file is done in a Python class and only the model solution runs on Dynare++.

The class is structured in 9 functions:
1. **__init__()**: initial values. 
2. **dict_parameters()**:  parameter dictionary
3. **dict_model()**: model definition
4. **mod_file()**: .mod file creation
5. **run_model()**: run model 
6. **key_variables()**: keys for plot
7. **plot_irf()**: IRF plot
8. **table_vcov()**: matrix of variance and covariance
9. **table_var()**: table of variance

The results are in `NKM_basic_model.ipynb`, it is structured in:
1. Introduction
2. Dynare model
3. Galí Chapter 3: $\theta=2/3$
4. Monetary, Technology and Phillips Curve shock with different $\theta$ values
5. Monetary, Technology and Phillips Curve shock with different $\theta$ values and without persistent shocks
6. Efficient interest rule
