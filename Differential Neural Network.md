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


[[Identification]]

Having an static neural network implies that for a given input pattern to such a static neural unit, an instantaneous output is obtained through a linear or nonlinear mapping procedure. A biological neuron not only contains a nonlinear mapping operation on the weighted sum of the input signals but also has some dynamic processes such as the state signal feedback, time delays, hysteresis and limit cycles. To emulate such a complex behavior, a number of dynamic or feedback neural units have been proposed.

```ad-info
The key distinction lies in whether the architecture of the neural network remains fixed (static) or can change dynamically during training (dynamic). Static networks are more common in traditional feedforward architectures, while dynamic networks are used when capturing temporal dependencies or sequential information is essential.

```
