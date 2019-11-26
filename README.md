# DeploymentGuide

## 01_MNIST_keras

In the folder 01_MNIST_keras can find a step by step about how to create a model (in keras) to classify numbers from MNIST database.

Also, there are in the folder, notebooks to save, freeze and optimize the model created with Keras and to load and test each one.

It is showed two tables, one with the mean time for the runs, and the second table is the mean time value divided by the batch size


## Performance 100 runs

Each model ran 100 times for each batch size, in the table is shown the mean time in ms


#### Entire batch 

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 1.9033 | 2.0848 | 2.3796 | 2.8857 | 5.4737 | 10.6925 | 20.8453
Frozen | 2.1116 | 1.6207 | 2.1041 | 2.6438 | 3.4164 | 4.5768 | 7.1868
Optimized | 2.1955 | 1.5326 | 1.7250 | 2.1402 | 2.8448 | 4.3492 | 6.9089

#### /batch size

Batch size | 4 | 8 | 16 | 32 | 64 | 128 | 256
--- | --- | --- | --- | --- | --- | --- | --- 
Model | 0.4758 | 0.2606 | 0.1487 | 0.0902 | 0.0855 | 0.0835 | 0.0814
Frozen | 0.5279 | 0.2026 | 0.1315 | 0.0826 | 0.0534 | 0.0358 | 0.0281
Optimized | 0.5489 | 0.1916 | 0.1078 | 0.0669 | 0.0445 | 0.0340 | 0.0270


## 01_MNIST_tensorflow

In the folder 01_MNIST_tensorflow can find a step by step about how to create a model (in TensorFlow) to classify numbers from MNIST database.

Also, there are in the folder, notebooks to save, freeze and optimize the model created with TensorFlow and to load and test each one.


## Performance 100 runs

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
