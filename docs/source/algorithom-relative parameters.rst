Algorithm-relative Parameter Desciption
=======================================
--init_method
-------------
 parameter initializers in the model

 * **normal**
 * **uniform**
 * **xavier_uniform**
 * **xavier_normal**

--optimizer       
-----------
 optimization algorithms in the model

 * **sgd**
 * **adam**
 * **adagrad**

--early_stop      
------------
 whether to activate early stop mechanism

--tune_testset
--------------
 whether to directly tune on testset

--factors
---------
 latent factors numbers in the model

--reg_1
-------
 L1 regularization

--reg_2
--------
 L2 regularization        

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
 number of layers in MLP model

--alpha
--------
 constant that multiplies the penalty terms in SLiM

--elastic
---------
 the ElasticNet mixing parameter in SLiM  

--pop-n
-------
 initial selected number of Most-popular in MostPop	  

--maxk
-------
 the (max) number of neighbors to take into account in ItemKNN

--node_dropout
--------------
 node dropout ratio in *NGCF* model

--mess_dropout
--------------
 mess dropout ratio in *NGCF* model

--kl_reg
---------
 Multi-VAE KL regularization