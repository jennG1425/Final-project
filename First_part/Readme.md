# Final-project _ First Part 
This is the first part of the final project of the Turbulence with AI subject with the professor [Dr. Guillermo Barrios] https://github.com/AltamarMx/ai_fluidmechanics. 

The work made with TBNN in this project is presented, first of all we give an introduction to TBNN, then we used a python code provided by [tbnn] https://github.com/tbnn/tbnn github repository, we proposed 3 changes in the original code. 

The chages were: 

|                   |    Original Code   |          Configuration 1          |          Configuration 2          |          Configuration 3          |
|:-----------------:|:------------------:|:---------------------------------:|:---------------------------------:|:---------------------------------:|
|       Layers      |          2         |                 1                 |                 10                |                 20                |
|       Nodes       |         20         |                 15                |                 20                |                 10                |
|  Maximum  epochs  |        2000        |                4000               |                5000               |                4000               |
|  Minimum  epochs  |        1000        |                2000               |                2000               |                1000               |
|  Split  fraction  |         0.8        |                0.8                |                0.9                |                0.7                |
| Jupyter  notebook | code_for_trainning | Code_for_training_1_Configuration | Code_for_training_2_Configuration | Code_for_training_3_Configuration |

In summary, we made 3 configurations in the first one we decreased the number of layers and in the other ones we increased to 10 and 20 layers and also we made changes in the number of neurons per layer, in some cases we decrease the neurons and in others we increase the nodes. 

The results obtained from the first configuration one compared to the others, showed that it is not necessary use more than 10 hidden layers with more than 15 neurons, because if we look for the graph, the original code and the one where we only decrease the layers to one, the results are too similar, so this show us, that adding more layers maybe is not necessary, because with that we are adding equations and operations that are not necessary. With this, we can conclude that to get an accurate result, we can use one or two layers with a range of 15 to 20 neurons per layer; if we want to use more than 10 layers, the results show us that we need to use less than 10 neurons because the difference between the real value and the prediction starts to grow.

---------------------------------------
## For the use of the TBNN
The package requires:
- Lasagne 0.2.dev1
- Theano 0.7.0.dev or above
- matplotlib 1.5.1 or above
- numpy 1.6.2 or above
- scipy 0.11 or above

And the to install, type: python setup.py install

## Bibliography

Ling,  J.,  Kurzawski,  A.,  Templeton,  J.,  2016.   Reynolds  averaged  turbulence  modelling  usingdeep  neural  networks  with  embedded  invariance.   Journal  of  Fluid  Mechanics  807,  155–166. doi:10.1017/jfm.2016.615

Milani,  P.M.,  Ling,  J.,  Eaton,  J.K.,  2019.   Tensor  Basis  Neural  Networks  for  Turbulent  ScalarFlux Modeling, in:  APS Division of Fluid Dynamics Meeting Abstracts, p. G17.002
