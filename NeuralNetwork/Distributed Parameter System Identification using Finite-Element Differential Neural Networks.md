#NeuralNetwork  #Rita

---


[[Non parametric Identification]] 

This article is about a method for [[Non parametric Identification]] of unknow  [[DPS]] using a [[DNN]]. Use [[PDEs]]

A [[DNN]] strcture is presented, in which borrowing some ideas from the finite element method allows the [[DNN]] to deal not only with ODEs but [[PDEs]] with 2D and 3D arbitrary domains.

A steady-state solution for the [[FEM]] is obtained by solving for $u$ in:

$$Ku=f$$
$K$ is the stiffness matrix
$f$ is correspondes to the source term in the [[PDEs]] or ODE that is being solved

The Neural Network uses the [[Sigmoid Function]]


> [!NOTE] Main Difference
> The main difference is that both $W_1$ and $V_1$ are assembled by using some ideas form the [[FEM]] allowing the identification of [[PDEs]] in two or three dimensions.
> 



