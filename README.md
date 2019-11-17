# DeploymentGuide

## 01_MNIST_keras_tf

In the folder 01_MNIST_keras_tf can find a step by step about how to create a model (in keras and TensorFlow) to classify numbers from MNIST database.

Also, there are in the folder, notebooks to save, freeze and optimize the model created with TensorFlow and to load and test each one.

* [01_MNIST_keras.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/01_MNIST_keras.ipynb) - create a model with Keras
* [02_00_MNIST_tensorflow.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_00_MNIST_tensorflow.ipynb) - create a model with TensorFlow
* [02_01_MNIST_save.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_01_MNIST_save.ipynb) - create a model with TensorFlow and save
* [02_02_MNIST_Freezing.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_02_MNIST_Freezing.ipynb) - Freeze the TensorFlow model created
* [02_03_MNIST_optimization.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_03_MNIST_optimization.ipynb) - Optimize the frozen model 
* [02_04_MNIST_load_model.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_04_MNIST_load_model.ipynb) - load, run and test the TensorFlow model created
* [02_05_MNIST_load_Frozen.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_05_MNIST_load_Frozen.ipynb) - load, run and test the frozen model
* [02_06_MNIST_load_optimized.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_06_MNIST_load_optimized.ipynb) - load, run and test the optimized model





### Performance 

Each model ran 100 times for each batch size, in the table is shown the mean time


Model | Batch size: 4 | Batch size: 8 | Batch size: 16 | Batch size: 32 | Batch size: 64 | Batch size: 128 | Batch size: 256
--- | --- | --- | --- | --- | --- | --- | --- 
Original | 1.8957 | 1.9569 | 2.3272 | 2.8502 | 3.2982 | 3.9983 | 6.3863
Frozen | 1.1339 | 1.0290 | 1.0152 | 1.0652 | 1.3136 | 1.7029 | 2.4653
Optimized | 1.7687 | 1.8855 | 1.9876 | 2.3957 | 3.0059 | 4.0875 | 6.7858

*time in ms


old

Model | Batch size: 4 | Batch size: 8 | Batch size: 16 | Batch size: 32 | Batch size: 64 | Batch size: 128 | Batch size: 256
--- | --- | --- | --- | --- | --- | --- | --- 
Original | 1.2044 | 1.0468 | 0.9961 | 1.0201 | 1.3075 | 1.6875 | 2.4400
Frozen | 1.9521 | 1.9812 | 2.4692 | 2.7717 | 3.2804 | 4.2291 | 7.1155
Optimized | 2.0656 | 2.0757 | 2.3632 | 2.8455 | 3.3992 | 4.0596 | 6.5692

*time in ms
