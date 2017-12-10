# neural-network
Handwritten digit recognition system trained on MNIST data. Taken from neuralnetworksanddeeplearning.com and updated to work with Python 3.6
This NN gives accuracy upto 95-96%. To get started, just clone or download the repo and run folowing commands:
		import mnist_loader
		training_data, validation_data, test_data = \
		mnist_loader.load_data_wrapper()
		import network
		net = network.Network([784, 30, 10])
		net.SGD(training_data, 30, 10, 3.0, test_data=test_data)
You can also chage the parameters in the last two lines to change the number of hidden networks (30 in the example) and number of epochs, batch size and learning rate (30, 10 and 3.0 respectively) in the final line as you prefer. You also need to change the address of the files in network.py.
