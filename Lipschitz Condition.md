In mathematical analysis, Lipschitz continuity, named after German mathematician Rudolf Lipschitz, is a strong form of uniform continuity for functions. Intuitively, a Lipschitz continuous function is limited in how fast it can change: there exists a real number such that, for every pair of points on the graph of this function, the absolute value of the slope of the line connecting them is not greater than this real number; the smallest such bound is called the Lipschitz constant of the function (and is related to the modulus of uniform continuity). 


> [!note]
>For instance, every function that is defined on an interval and has bounded first derivative is Lipschitz continuous. 



Given two metric spaces $(X, d_X)$ and $(Y, d_Y)$, where $(d_X)$ denotes the metric on the set $(X)$ and $(d_Y)$ is the metric on set $(Y)$, a function $(f : X \to Y)$ is called Lipschitz continuous if there exists a real constant \(K \geq 0\) such that, for all $(x_1)$ and $(x_2)$ in $(X)$,

$$d_Y(f(x_1), f(x_2)) \leq K d_X(x_1, x_2)$$

Any such $K$ is referred to as a Lipschitz constant for the function $f$ and $f$ may also be referred to as $K$-Lipschitz. The smallest constant is sometimes called the (best) Lipschitz constant of $f$ or the dilation or dilatation of $f$.

If $(K = 1)$ the function is called a short map, and if $0 \leq K < 1$ and $f$ maps a metric space to itself, the function is called a contraction.

In particular, a real-valued function $f : \mathbb{R} \to \mathbb{R}$ is called Lipschitz continuous if there exists a positive real constant $K$ such that, for all real $x_1$ and $x_2$,

$$|f(x_1) - f(x_2)| \leq K |x_1 - x_2|$$

In this case, $Y$ is the set of real numbers $mathbb{R}$ with the standard metric $d_Y(y_1, y_2) = |y_1 - y_2|$, and $X$ is a subset of $\mathbb{R}$
