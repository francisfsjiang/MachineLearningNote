# One Variable

* m = Number of training examples.
* x = "input" variable / feature.
* y = "output" variable / "target" variable.

Hypothesis

$$ h_{\theta} (x) = \theta_0 + \theta_1 x$$

Parameters

$$ \theta_0, \theta_1$$

CostFunction

$$J (\theta_0, \theta_1) = \frac{1}{2 m} \sum_{i = 1}^{m_{}} (h_{\theta}
(x^{(i)}) - y^{(i)})^2$$

$$\underset{\theta_0, \theta_1}{minimize}  J (\theta_0, \theta_1)$$


$$\begin{array}{lll}
  \theta_j & = & \theta_j - \alpha \frac{\partial}{\partial \theta_j} J
  (\theta_0, \theta_1)  (for j = 0 and j = 1)
\end{array}$$

$$\begin{array}{lll}
  temp_0 & = & \theta_0 - \alpha \frac{d}{d \theta_0} J (\theta_0,
  \theta_1)\\
  temp_1 & = & \theta_1 - \alpha \frac{d}{d \theta_1} J (\theta_0,
  \theta_1)\\
  \theta_0 & = & temp_0\\
  \theta_1 & = & temp_1
\end{array}$$