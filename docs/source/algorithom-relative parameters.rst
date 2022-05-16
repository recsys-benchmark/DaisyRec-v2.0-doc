Algorithm-relative Parameter Desciption Format1
================================================

init_method
------------
   Parameter initializers in the model.

optimizer
----------
   Optimization algorithms in the model.

early_stop
----------
   Whether to activate early stop mechanism.

tune_testset
------------
   Whether to directly tune on testset.

factors
-------
   Latent factors numbers in the model.

reg_1
-----
   L1 regularization.

reg_2
-----
   L2 regularization.

dropout
-------
   Dropout rate.

lr
-----
   Learning rate.

epochs
--------
   Training epochs.

batch_size
-----------
   Batch size for training.

num_layers
-----------
   Number of layers in MLP model.

alpha
-----
   Number of layers in MLP model.

elastic
-------
   Constant that multiplies the penalty terms in SLiM.

pop-n
-----
   	Initial selected number of Most-popular in MostPop.

maxk
-----
   The (max) number of neighbors to take into account in ItemKNN.

node_dropout
---------------
   Node dropout ratio in NGCF.

mess_dropout
-------------
   Mess dropout ratio in NGCF.

kl_reg
------
   VAE KL regularization.


Algorithm-relative Parameter Desciption Format2
=================================================

--init_method     parameter initializers in the model
--optimizer       optimization algorithms in the model
--early_stop      whether to activate early stop mechanism
--tune_testset    whether to directly tune on testset
--factors         latent factors numbers in the model
--reg_1           L1 regularization
--reg_2           L2 regularization
--dropout         dropout rate
--lr              learning rate
--epochs          training epochs
--batch_size      batch size for training
--num_layers      number of layers in MLP model
--alpha           constant that multiplies the penalty 
                  terms in SLiM
--elastic         the ElasticNet mixing parameter in SLiM
--pop-n	         initial selected number of Most-popular in MostPop
--maxk            the (max) number of neighbors to take into account 
                  in ItemKNN
--node_dropout    node dropout ratio in *NGCF* model
--mess_dropout    mess dropout ratio in *NGCF* model
--kl_reg          VAE KL regularization