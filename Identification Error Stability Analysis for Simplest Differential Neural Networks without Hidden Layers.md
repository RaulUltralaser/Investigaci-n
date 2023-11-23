The nonlinear system to be identified is given as:

$$\begin{align}\dot{x}_t&=f(x_t,u_t,t)\\x_t&\in\mathbb{R}^n,u_t\in\mathbb{R}_q, n\geq q\end{align}$$

We assume the following parallel structure of neural networks
$$\dot{\hat{x}}=A\hat{x}_t+W_{1,t}\sigma(\hat{x}_t)+W_{2,t}\phi(\hat{x}_t)\gamma(u_t)$$
where


$$\begin{align}\hat{x}_t&\in\mathbb{R}^n\\u_t&\in\mathbb{R}^q\\W_{1,t}&\in\mathbb{R}^{n\times k}\\W_{2,t}&\in\mathbb{R}^{n\times r}\\A&\in\mathbb{R}^{n\times n}\end{align}$$
Are
1) the state of the neural network
2) an input measurable control action
3) is the matrix for nonlinear state feedback
4) is the input matrix
5) is a Hurtwitz matrix

and $\sigma_i()$, $\phi_{ij}()$ are sigmoid functions
$$\begin{align}\sigma_i(x)&=a_i(1+e^{-b_ix_i})^{-1}-c_i\\\phi_{ij}(x)&=\bar{a}_{ij}(1+e^{-\sum_p\bar{b}_{ij}^px^p})^{-1}-\bar{c}_{ij}\end{align}$$
