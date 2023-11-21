```ad-question
Can the dynamic systems under consideration be adequately represented within a given particular model structure?

```

Identifiability on neural networks is related to uniqueness of the weights and to whether two networks with different parameter can produce identical input/output behavior

A straightforward approach is to augment the networks inputs with signals corresponding to its inputs and outpus. Assuming that the nonlinear system is described by:

$$y(k+1)=g(y(k),y(k-1)...y(k-n),u(k),u(k-1)...u(k-m))$$
$$y,u\in \mathbb{R}, m<n$$
where $y$ depends linearly on either its past values or on those of $u$

An obvious approach to model the system is to select the input-output structure of a the neural network to be the same as that of the system. Denoting the output of the neural network as $y_{nn}$ then there exist two possible implementation.

*a) series parallel model*
The system output are used as the inputs of the neural network
$$y_{nn}(k+1)=g(y(k),y(k-1)...y(k-n),u(k),u(k-1)...u(k-m))$$
Because there is not recurrence in the equation this correspond to a **static neural network.**

*b) parallel model *

Here past outputs of the neural network are used as component of its input

$$y_{nn}(k+1)=g(y_{nn}(k),y_{nn}(k-1)...y_{nn}(k-n),u(k),u(k-1)...u(k-m))$$
Because of the recurrence of $y_{nn}$ in this equation, this correspond to a **dynamic neural network.**

Once the structure is defined, the next step is to determine the learning algorithm. 

The simplest approach is to introduce a training signal to the system and to use the system output as the input to the neural network, whose output is compare with the training signal; the respective error is used to train the neural network.

The input-output approach is not easily extended to multi-input, multi-output approach. For these cases is better to use a state space representation. Given the nonlinear system:
$$\begin{align}x(k+1)&=f(x(k),u(k))\\y(k)&=h(x(k))\\x\in\mathbb{R}^n,u\}\in&\mathbb{R}^m,y\in\mathbb{R}^l,k=0,1,...\end{align}$$

The following neural network identifier is proposed:

$$\begin{align}x_{nn}(k+1)&=W_1\varphi(V_ax_{nn}(k)+V_bu(k)+\rho_x+Ke(k)\\y_{nn}(k)&=W_2\varphi(V_cx_{nn}(k)+V_du(k)+\rho_y)\\e(k)&=y(k)-y_{nn}(k),x(0)=x_{nn}(0)\end{align}$$


