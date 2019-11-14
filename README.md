# DeploymentGuide

## 01_MNIST_keras_tf

In the folder 01_MNIST_keras_tf can find a step by step of how to create a model (in keras and TensorFlow) to classify numbers from MNIST database.

Also, there are in the folder, notebooks to save, freeze and optimize the model created with TensorFlow and to load and test each one.

* [01_MNIST_keras.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/01_MNIST_keras.ipynb) - create a model with Keras
* [02_00_MNIST_tensorflow.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_00_MNIST_tensorflow.ipynb) - create a model with TensorFlow
* [02_01_MNIST_save.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_01_MNIST_save.ipynb) - create a model with TensorFlow and save
* [02_02_MNIST_Freezing.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_02_MNIST_Freezing.ipynb) - Freeze the TensorFlow model created
* [02_03_MNIST_optimization.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_03_MNIST_optimization.ipynb) - Optimize the frozen model 
* [02_04_MNIST_load_model.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_04_MNIST_load_model.ipynb) - load, run and test the TensorFlow model created
* [02_05_MNIST_load_Frozen.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_05_MNIST_load_Frozen.ipynb) - load, run and test the frozen model
* [02_06_MNIST_load_optimized.ipynb](https://github.com/joseruiz1989/DeploymentGuide/blob/master/01_MNIST_keras_tf/02_06_MNIST_load_optimized.ipynb) - load, run and test the optimized model


time average in ms for the TensorFlow models

batch 4: 100 runs with batch of 4

batch 1000: 1000 runs with batch of 1000


Time in ms | batch: 4 | batch: 1000
--- | --- | --- 
model | 1.9872 | 21.357 
frozen | 1.2127 | 6.9343 
optimized | 1.2175 | 6.5938 
