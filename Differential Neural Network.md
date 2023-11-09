#NeuralNetwork #Rita 
_____
The neuron is the fundamental unit for the operation of a neural network presents a neuron scheme. There are three basic elements:

1.-A set of synapsis links, with each element characterized by its own weight.

2.- An adder for summing the inputs signal components, multiplied by the respective synapsis weight.

3.-A nonlinear activation function transforming the adder output into the output of the neuron.

An *external threshold* is also applied to lower the input to the activation function. In mathematical terms, the $i-th$ neuron can be described as:

$$v_i=\sum^n_{j=1} w_{ij}u_j$$

$$y_i=\varphi(v_i-\rho_i)$$
where: 
$u_j$ is the $j-th$ component of the input
$\omega_{ij}$ is the weight connecting the $j-th$ input component to neuron $i$
$v_i$ is the output of the adder,
$\rho_i$ is the threshold
$\varphi(.)$ is the nonlinear activation function,
$y_i$ is the output of neuron $i$
