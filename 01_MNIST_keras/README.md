# DeploymentGuide - 01_MNIST_keras

In the folder 01_MNIST_keras can find a step by step about how to create a model (in keras) to classify numbers from MNIST database.

Also, there are in the folder, notebooks to save, freeze and optimize the model created with Keras and to load and test each one.

* [01_00_MNIST_keras_create_save_freeze_optimize.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras/01_00_MNIST_keras_create_save_freeze_optimize.ipynb) - create a model with Keras, save, freeze and optimize it
* [01_01_MNIST_keras_load_model_frozen_optimized.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras/01_01_MNIST_keras_load_model_frozen_optimized.ipynb) - load the created, frozen and optimized models, perform inferences with each one


## Performance 100 runs

Each model ran 100 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Barch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 2.2344 | 2.2516 | 2.7749 | 3.1151 | 6.0261 | 10.9382 | 21.1812
Frozen | 2.3201 | 1.9666 | 2.0530 | 2.6303 | 3.4813 | 5.0470 | 7.0212
Optimized | 1.8006 | 1.1277 | 1.0676 | 1.2247 | 1.3855 | 1.6140 | 2.5119

#### /batch size

Barch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.5586 | 0.2814 | 0.1734 | 0.0973 | 0.0942 | 0.0855 | 0.0827
Frozen | 0.5800 | 0.2458 | 0.1283 | 0.0822 | 0.0544 | 0.0394 | 0.0274
Optimized | 0.4502 | 0.1410 | 0.0667 | 0.0383 | 0.0216 | 0.0126 | 0.0098


## Performance 100 runs in one file

Each model ran 100 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Barch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 1.9033 | 2.0848 | 2.3796 | 2.8857 | 5.4737 | 10.6925 | 20.8453
Frozen | 2.1116 | 1.6207 | 2.1041 | 2.6438 | 3.4164 | 4.5768 | 7.1868
Optimized | 2.1955 | 1.5326 | 1.7250 | 2.1402 | 2.8448 | 4.3492 | 6.9089

#### /batch size

Barch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.4758 | 0.2606 | 0.1487 | 0.0902 | 0.0855 | 0.0835 | 0.0814
Frozen | 0.5279 | 0.2026 | 0.1315 | 0.0826 | 0.0534 | 0.0358 | 0.0281
Optimized | 0.5489 | 0.1916 | 0.1078 | 0.0669 | 0.0445 | 0.0340 | 0.0270




## Performance 10000 runs in one file

Each model ran 10000 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Barch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 1.8605 | 1.9962 | 2.3900 | 2.8927 | 5.4102 | 10.4648 | 20.6492
Frozen | 1.5740 | 1.7225 | 2.0337 | 2.5568 | 2.8283 | 4.2043 | 7.1537
Optimized | 1.6471 | 1.7330 | 2.0437 | 2.5582 | 2.8110 | 4.2355 | 7.1992

#### /batch size

Barch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.4651 | 0.2495 | 0.1494 | 0.0904 | 0.0845 | 0.0818 | 0.0807
Frozen | 0.3935 | 0.2153 | 0.1271 | 0.0799 | 0.0442 | 0.0328 | 0.0279
Optimized | 0.4118 | 0.2166 | 0.1277 | 0.0799 | 0.0439 | 0.0331 | 0.0281


