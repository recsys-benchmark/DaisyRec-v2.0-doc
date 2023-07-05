Basic Settings
============================
--problem_type
--------------
  define a point-wise or pair-wise problem.

  * **point-wise**: point-wise algorithm
  * **pair-wise**: pair-wise algorithm

--optimization_metric
---------------------
  the metric to be optimized for hyper-parameter tuning via HyperOpt
  
  * **ndcg**
  * **precision**
  * **recall**
  * **hr**
  * **map**
  * **mrr**

--hyperopt_trail
-----------------
  the number of trails of HyperOpt

--hyperopt_pack
---------------
  record the searching space of hyper-parameters for HyperOpt

--algo_name
------------
  the algorithm to be executed

  * **mostpop**
  * **itemknn**
  * **puresvd**
  * **slim**
  * **mf**
  * **fm**
  * **neumf**
  * **nfm**
  * **ngcf**
  * **multi-vae**

--dataset
----------
  the dataset to be evaluated 
  
  * **ml-100k**
  * **ml-1m**
  * **ml-10m**
  * **ml-20m**
  * **lastfm**
  * **book-x**
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
  the data pre-processing strategy
  
  * **origin**: adopt the raw data
  * **Fcore**: recursively filter users and items that have interactions no less than N, e.g., 5core
  * **Ffilter**: only filter users and items that have interactions no less than N once, e.g., 5filter
  
--val_method
-------------
  training and validation data splitting strategy

  * **tsbr**: time-aware split-by-ratio
  * **rsbr**: random-aware split-by-ratio
  * **tloo**: time-aware leave-one-out
  * **rloo**: random-aware leave-one-out

--test_method
--------------
  training and test data splitting strategy, which should be consistent with the settings for **val_method**

--val_size
-----------
  ratio of validation set size in the range of (0,1), e.g., 0.1 means retaining 10% of training data as validation data

--test_size
-----------
  ratio of test set size in the range of (0,1), e.g., 0.2 means retaining 20% of the whole data as test data

--topk
-------
  the length of recommendation list

--fold_num
----------
  the fold number of cross-validation

--cand_num
----------
  the number of candidate items used for ranking

--sample_method
---------------
 negative sampling strategy

 * **uniform**: uniformly sample negative items
 * **low-pop**: sample popular items with low rank
 * **high-pop**: sample popular items with high rank

--sample_ratio
--------------
  control the ratio of popularity sampling for the hybrid sampling strategy in the range of (0,1), e.g., for the hybrid sampling strategy uniform+low-pop, --sample_ratio=0.1 means 10% of the negative items are sampled via low-pop 

--num_ng
--------
  the number of negative samples

--positive_threshold
--------
  the threshold for binarizing the ratings into positve samples (for exmaple if the threshold = 4, it means the items with ratings no less than 4 will be treated as positive items)

--loss_type
-----------
  type of loss function

  * **CL**: cross-entropy loss for point-wise problem
  * **SL**: square error loss for point-wise problem
  * **BPR**: BPR loss for pair-wise problem
  * **HL**: hinge loss for pair-wise problem
  * **TL**: top-1 Loss for pair-wise problem

--gpu
-----
  the ID of GPU card
