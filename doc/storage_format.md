# HDF5 data format

## Parameter estimation settings
Parameter estimation settings are saved in `/optimization_settings`.

## Parameter estimation results
Parameter estimation results are saved in `/optimize_results/`.

### Results per local optimization
Results of the `$n`'th multistart a saved in the format
```
+ /optimization_results/multistarts/$n/
  - fval: Objective function value of best iteration
  - x: Parameter set of best iteration
  - grad: Gradient of objective function at point x
  - hess: Hessian matrix of objective function at point x
  - n_fval: Total number of objective function evaluations
  - n_grad: Number of gradient evaluations
  - n_hess: Number of Hessian evaluations
  - n_res: Number of residual evaulations
  - n_sres: Number of residual sensitivity evaluations.
  - x0: Initial parameter set
  - fval0: Objective function value at starting parameters
  - exitflag: ...
  - time: ...
  - message: ...
```
The history is saved under `/optimization_results/multistarts/$n/trace/`

## Sampling results

TODO