Confider a setting in which the feature variables are mean centered, but the mean of the binary class prediction from $\{-1,+1\}$ is not $0$. This will tend to occur in situations in which the binary class distribution is highly imbalanced. In such case, the aforementioned approach is not sufficient for prediction. We need to incorporate an additional bias variable $b$ that captures this invariant part of the prediction:

$$\hat{y}=sign{\bar{W}\bar{X}+b}=sign{\sum_{i=1}^{d}w_ix_i+b}$$

