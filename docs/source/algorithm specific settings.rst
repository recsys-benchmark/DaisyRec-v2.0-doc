Algorithm Specific Settings
=======================================
--init_method
-------------
 parameter initializers

 * **normal**: initialize parameters with normal distribution
 * **uniform**: initialize parameters with uniform distribution
 * **xavier_normal**: initialize parameters with xavier_normal distribution
 * **xavier_uniform**: initialize parameters with xavier_uniform distribution

--optimizer       
-----------
 optimization method for training the algorithms

 * **sgd**
 * **adam**
 * **adagrad**

--early_stop      
------------
 whether to activate the early-stop mechanism

 * **true**
 * **false**

--tune_testset
--------------
 whether to directly tune on testset, and the default value is false

 * **true**
 * **false**
  
--factors
---------
 the dimension of latent factors (embeddings)

--reg_1
-------
 the coefficient of L1 regularization

--reg_2
--------
 the coefficient of L2 regularization        

--dropout
----------
 dropout rate

--lr
----
 learning rate

--epochs
--------
 training epochs

--batch_size
------------
 batch size for training

--num_layers
------------
 number of layers for MLP

--alpha
--------
 constant to multiply the penalty terms for SLIM

--elastic
---------
 the ElasticNet mixing parameter for SLIM in the range of (0,1)  

--pop-n
-------
 the preliminary selected top-n popular candidate items to reduce the time complexity for MostPop	  

--maxk
-------
 the number of neighbors to take into account for ItemKNN

--node_dropout
--------------
 node dropout ratio for NGCF

--mess_dropout
--------------
 message dropout ratio for NGCF 

--kl_reg
---------
 the coefficient of KL regularization for Multi-VAE