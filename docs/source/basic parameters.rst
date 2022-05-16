Basic Parameters Description
============================
--problem_type
--------------
  Define a point-wise or pair-wise algorithm.

  * **point**: point-wise algorithm
  * **pair**: pair-wise algorithm

--score_metric
--------------
  Metric to define hyperopt score.
  
  * **ndcg**
  * **precision**
  * **recall**
  * **hr**
  * **map**
  * **mrr**

--tune_epochs
-------------
  Epoch number to tune an algorithm.

--tune_pack
------------
  The parameter that Hyperopt need tp pass, this will automatically generate by GUI.

--algo_name
------------
  Name of algorithm that need to implement.

  * **mostpop**
  * **itemknn**
  * **puresvd**
  * **slim**
  * **bprmf**
  * **bprfm**
  * **neumf**
  * **nfm**
  * **ngcf**
  * **vae**

--dataset
----------
  The selected datasets.
  
  * **ml-100k**
  * **ml-1m**
  * **ml-10m**
  * **ml-20m**
  * **lastfm**
  * **bx**
  * **amazon-cloth**
  * **amazon-electronic**
  * **amazon-book**
  * **amazon-music**
  * **epinions**
  * **yelp**
  * **citeulike**
  * **netflix**

--prepro
---------
  The data pre-processing method.
  
  * **origin**: origin means using the raw data
  * **Ncore**: Ncore means only preserving users and items that have interactions more than N. Notice N could be any integer value.
  * **Nfilter**: Nfilter only filter users or items that have interactions more than N
  
--val_method
-------------
  Train-validation splitting.

  * **tsbr**: time-aware split-by-ratio
  * **rsbr**: random-aware split-by-ratio
  * **tloo**: time-aware leave-one-out
  * **rloo**: random-aware leave-one-out

--test_method
--------------
  Train-test splitting. The parameter is same with **val_method**

--topk
-------
  The length of recommendation list.

--test_size
-----------
  Ratio of test set size

--val_size
----------
  Ratio of validation set size

--fold_num
----------
  The number of fold used for validation.

--cand_num
----------
  The number of candidate items used for ranking.

--sample_method
---------------
  Negative sampling method.

* **uniform**: uniformly sampling
* **item-ascd**: sampling popular items with low rank
* **item-desc**: sampling popular items with high rank

--sample_ratio
--------------
  Mix sample method ratio, 0 for all uniform.

--num_ng
--------
  The number of negative samples.

--loss_type
------------
  Type of loss function.

  * **CL**: Cross-entropy loss for point-wise problem
  * **SL**: Square loss for point-wise problem
  * **BPR**: BPR loss for pair-wise problem
  * **HL**: Hinge loss for pair-wise problem
  * **TL**: Top-1 Loss for pair-wise problem

--gpu
------
  The GPU card ID
