#Rita #NeuralNetwork 
___ 
The neurons are connected to other neurons with axons or dendrites, and the connecting regions between axons and dendrites are referred to as synapses.

Deep learners become more attractive than conventional methods primarily when sufficient data/computational power is available.

The performance of traditional machine learning remains better at times for smaller data sets.

[[Perceptron]]

[[Bias]]

[[Activation Functions]]

[[Backpropagation]]

In spite of the formidable reputation of neural networks as universal function approximators, considerable challenges remain with respect to actually training neural networks to provide this level of performance. 

[[The problem of Overfitting]]


> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"_index":0}] Theorem 1.
> A multi-layer network that uses only the identity activation function in all its layers reduces to a  single-layer network performing linear regression.


> [!math|{"type":"lemma","number":"auto","setAsNoteMathLink":false,"_index":1}] Lemma 2.
> Consider a multilayer network in which all hidden layers use identity activation and the single output node uses the perceptron criterion as the loss function and the sign activation for prediction. This neural network reduces to the single-layer perceptron


This is the reason to gain depth with nonlinear activation function in the hidden layers.