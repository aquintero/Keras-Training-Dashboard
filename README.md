# Keras-Training-Dashboard
A dashboard to aid the iteration process of designing neural network architectures.

##Feature Goals

###Design Phase
* Show editable graph of network layers and output shapes between layers. Include visualizations for:
    * number of number of parameters at each layer
    * expected computational resources required at each layer
    * representational bottlenecks (e.g. strided pooling, reduced filter bank)
* Initial layers to be supported
    * Dense
    * Convolution
    * Dropout
* Define hyper parameters for monitoring or tuning. Some potential examples:
    * the inclusion of a layer
    * number of filters of a layer
    * other layer parameters
    * optimization methods (SGD, adagrad, adadelta, etc.)
    * loss function
    * types of data augmentation
    * types of data normalization
* Data feeding (define train, validation, and test sets)
* Data augmentation (flips, rotations, crops, noise)
* Visualize data
    * histogram of labels
    * outlier analysis
    * query individual samples
* Define loss function mse, (binary cross-entropy, categorical cross_entropy etc.)
* Define optimization method (SGD, adagrad, adadelta, etc.)
* Define initialization method (e.g. glorot_uniform)
* Define metrics (predicted R^2, accuracy, precision, recall, f_beta, etc.)
* Define training parameters (epochs, batch size, class_weights, etc.)

###Training Phase
* Show training metrics
* View network inputs during training
    * query for individual training samples
    * display overall data visualization and statistics.
* Visualize network layers (between epochs?)
    * conv layers showing filter list
    * dropout showing disconnected sections?
* Visualize metrics/loss and compare validation curves

###Testing Phase
* Visualize history of results along with network architectures and hyperparameter values.
* Visualize conv layers as maximum activation from an image.
* Visualize result statistics on different labels
