| Options | Description|
|---|---|
|**`--nodes`**|      The number of nodes per hidden layer in the neural network|
|**`--N0`** |               The number of points to use on the initial condition|
|**`--Nb`** |               The number of points to use on the boundary condition|
|**`--Nf`** |             The number of collocation points to use||
|**`--epochs`**|       The number of epochs to train the neural network|
|**`--display-freq`**|  How often to display loss information|
|**`--layers`**| The number of hidden layers in the neural network|
|**`--method`**| Sampling method|

The weights for the IC, BC, and PDE residual losses are set to 1, 1, and 1, respectively.

The available sampling methods include 'fixed', 'random-r', 'rad', 'r3', 'l_inf', and 'las'. In cases where hyperparameter settings are required for each method, the default settings from the original paper have been applied. If modifications are necessary, these should be made within the code. For instance, in 'rad', set k=c=1, and in 'l_inf', set the number of iterations to 20.

###### Our PINN training and evaluation implementation is built upon the work presented in https://github.com/CVC-Lab/RobustPINNs
