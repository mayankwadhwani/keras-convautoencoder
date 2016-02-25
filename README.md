# Keras autoencoders (convolutional/fcc)
This is an implementation of weight-tieing layers that can be used to consturct convolutional autoencoder and 
simple fully connected autoencoder. It might feel be a bit hacky towards, however it does the job.

## Convolutional autoencoder [CAE] example 
l
Run conv_autoencoder.py.
Conv layer (32 kern of 3x3) -> MaxPool (2x2) -> Dense (10) -> DePool (2x2) -> DeConv layer (32 kern of 3x3)
Weights of Conv and Deconv layers are tied;
MaxPool and DePool shares activated neurons. 
![ConvAutoEncoder MNIST representations](./img/cc.png "ConvAutoEncoder MNIST representations")

## FCC autoencoder example

Run fcc_autoencoder.py.
FСС (50) -> FСС (30) -> FСС (30) -> FСС (50)
![FСС MNIST representations](./img/fcc.png "ConvAutoEncoder MNIST representations")

## ConvAutoEncoder on 1100 cars 

![ConvAutoEncoder cars representations](./img/cars.png "ConvAutoEncoder cars representations")
