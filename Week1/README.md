## Mathematics for Gradient Descent

Assuming a linear model of the form <img src="https://latex.codecogs.com/gif.latex?\hat{y}=b_{0}+b_{1}x"/> and a dataset <img src="https://latex.codecogs.com/gif.latex?[(x_{1},y_{1}),(x_{2},y_{2}),(x_{3},y_{3}),...,(x_{n},y_{n})]"/>. 

Using the following loss function:

<img src="https://latex.codecogs.com/gif.latex?L(b_{0},b_{1})=\sum_{i=1}^{n}(\hat{y_{i}}-y_{i})^{2}+\lambda.b_{1}^{2}"/>, where <img src="https://latex.codecogs.com/gif.latex?\lambda>0"/> 

the objective is to derive the best values by solving the following set of equations: 

- <img src="https://latex.codecogs.com/gif.latex?dL/db_{0}=0"/>
- <img src="https://latex.codecogs.com/gif.latex?dL/db_{1}=0"/>

### Solution

<img src="/images/big-data-analytics/gradient-descent-math.png?raw=true"/>
