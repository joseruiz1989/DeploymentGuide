# DeploymentGuide - 01_MNIST_tensorflow

In the folder 01_MNIST_tensorflow can find a step by step about how to create a model (in TensorFlow) to classify numbers from MNIST database.

Also, there are in the folder, notebooks to save, freeze and optimize the model created with TensorFlow and to load and test each one.

* [01_00_MNIST_tf_create_save_freeze_optimize.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_tensorflow/01_00_MNIST_tf_create_save_freeze_optimize.ipynb) - create a model with TensorFlow, save, freeze and optimize it
* [01_01_MNIST_tf_load_model_frozen_optimized.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_tensorflow/01_01_MNIST_tf_load_model_frozen_optimized.ipynb) - load the created, frozen and optimized models, perform inferences with each one


It is showed two tables, one with the mean time for the runs, and the second table is the mean time value divided by the batch size


## Performance 100 runs

Each model ran 100 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 1.0932 | 1.1129 | 1.1155 | 1.2070 | 1.3466 | 1.7530 | 2.5127
Frozen | 1.2710 | 1.0912 | 1.0977 | 1.2155 | 1.4310 | 1.7698 | 2.4858
Optimized | 2.0240 | 2.1458 | 2.5314 | 2.8266 | 3.4124 | 4.3743 | 7.0463

#### /batch size

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.2733 | 0.1391 | 0.0697 | 0.0377 | 0.0210 | 0.0137 | 0.0098
Frozen | 0.3178 | 0.1364 | 0.0686 | 0.0380 | 0.0224 | 0.0138 | 0.0097
Optimized | 0.5060 | 0.2682 | 0.1582 | 0.0883 | 0.0533 | 0.0342 | 0.0275


## Performance 100 runs in one file

Each model ran 100 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 2.2705 | 2.2624 | 2.6087 | 2.9381 | 3.6173 | 4.4693 | 7.6755
Frozen | 2.7985 | 1.7355 | 1.9956 | 2.3808 | 2.9216 | 4.0797 | 7.1339
Optimized | 2.9318 | 1.6503 | 2.0097 | 2.2474 | 2.9278 | 4.0801 | 7.1074

#### /batch size

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.5676 | 0.2828 | 0.1630 | 0.0918 | 0.0565 | 0.0349 | 0.0300
Frozen | 0.6996 | 0.2169 | 0.1247 | 0.0744 | 0.0456 | 0.0319 | 0.0279
Optimized | 0.7329 | 0.2063 | 0.1256 | 0.0702 | 0.0457 | 0.0319 | 0.0278




## Performance 10000 runs in one file

Each model ran 10000 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 1.8040 | 1.8947 | 2.2451 | 2.3267 | 2.7722 | 4.1596 | 6.9335
Frozen | 1.8153 | 1.9210 | 2.2805 | 2.4357 | 2.7932 | 4.1487 | 6.9425
Optimized | 1.7941 | 1.9088 | 2.2841 | 2.3861 | 2.7854 | 4.1323 | 6.9143

#### /batch size

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.4510 | 0.2368 | 0.1403 | 0.0727 | 0.0433 | 0.0325 | 0.0271
Frozen | 0.4538 | 0.2401 | 0.1425 | 0.0761 | 0.0436 | 0.0324 | 0.0271
Optimized | 0.4485 | 0.2386 | 0.1428 | 0.0746 | 0.0435 | 0.0323 | 0.0270




## Performance 1000 runs in one file

Each model ran 1000 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 1.8552 | 1.9418 | 2.2734 | 2.5480 | 2.8355 | 4.2212 | 7.1293
Frozen | 1.7526 | 1.7850 | 2.1534 | 2.4851 | 2.8010 | 4.2102 | 7.1131
Optimized | 1.6663 | 1.6470 | 1.9141 | 2.2412 | 2.7408 | 4.1173 | 7.1203

#### /batch size

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.4638 | 0.2427 | 0.1421 | 0.0796 | 0.0443 | 0.0330 | 0.0278
Frozen | 0.4381 | 0.2231 | 0.1346 | 0.0777 | 0.0438 | 0.0329 | 0.0278
Optimized | 0.4166 | 0.2059 | 0.1196 | 0.0700 | 0.0428 | 0.0322 | 0.0278
