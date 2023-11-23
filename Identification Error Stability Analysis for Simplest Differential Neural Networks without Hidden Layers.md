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
This Neural Network can be classified  as a Hopfield-type one.

> [!math|{"type":"theorem","number":"auto","setAsNoteMathLink":false,"_index":0}] Theorem 1.
> Let us consider the unknown nonlinear system as the first equation and a mode matching neural network as the second equation whose weights are adjusted as 
> $$\begin{align}\dot{W}_{1,t}&=-K_1P\Delta_t\sigma(\hat{x}_t)^T\\\dot{W}_{2,t}&=-K_2P\Delta_t\gamma(u_t)\phi(\hat{x}_t)^T\end{align}$$
> with $W_{1,0},W_{2,0}$ the initial weight matrices. $K_1$,$K_2$ are positive defined matrices, $P$ is the solution of matrix Riccati equation. Assume also that the assumptions **A2.1, A2.2 and A2.3** hold. Then the weights dynamics are bounded:
> $$W_{1,t}\in L_\infty, W_{2,t}\in L_\infty$$
> and converge
> $$\lim_{t\rightarrow \infty}\dot{W}_{1,t}=0,\lim_{t\rightarrow \infty}\dot{W}_{2,t}=0$$
> we also can conclude that the identification process is asymptotically consistent, i.e. 
> $$\lim_{t\rightarrow \infty}\Delta_t=0$$

