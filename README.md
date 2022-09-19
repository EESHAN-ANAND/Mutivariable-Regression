# Mutivariable-Regression
**The implementation of multivariable regression is done in the given repository**

**Multivariable Regression:-** Multivariable regression models are used to establish the relationship between a dependent variable and *more than 1 independent variable*. Multivariable regression can be used for a variety of different purposes in research studies.

Multivariate Regression is a supervised machine learning algorithm which is used to provide prediction based on continuous valued feature.

So lets say that we are training our data based on m points and we are training our model based on n features, then just because we want to establish an optimum linear relation between the independent variable and dependent variable (here acts as y), our y*predicted* can be defined for each point as:-![image](https://user-images.githubusercontent.com/113720338/191075797-8c26352c-7922-4665-a911-b9e5dd533e42.png)

And our *ytrue* can be defined as(here e defined the error matrix):-
![image](https://user-images.githubusercontent.com/113720338/191075274-a6d7ab7c-3cab-4c5b-957f-d4425dfd0d48.png)

The error can be ignored as the data is inpredictable and inconsistent (as always!!) and the coefficients can be calcualated by matrix multiplication method but the **cost of finding the coefficients is very costly and the time complexity increases rapidly as the feature increases**. So we used *gradient descent*.

**Gradient Descent** :-Gradient Descent is known as one of the most commonly used optimization algorithms to train machine learning models by means of minimizing errors between actual and expected results. Further, gradient descent is also used to train Neural Networks.

In mathematical terminology, Optimization algorithm refers to the task of minimizing/maximizing an objective function f(x) parameterized by x. Similarly, in machine learning, optimization is the task of minimizing the cost function parameterized by the model's parameters. The main objective of gradient descent is to minimize the convex function using iteration of parameter updates. Once these machine learning models are optimized, these models can be used as powerful tools for Artificial Intelligence and various computer science applications.

So we do is take the partial derivative of cost with respect to a coefficient of feature i (m*i*) and plot the graph of cost with respect to mi. So the aim is to reach the mimima of the cost as much as possible, so we start from a value in the coefficient and constantly iterate it for n number of time to reach minima. That's how we actually determine optimum coefficient for each variable.
![image](https://user-images.githubusercontent.com/113720338/191079684-64ac7ae7-2776-4baf-b8be-33d29e2de4b1.png)
[Credit-javapoint.com](https://www.javatpoint.com/gradient-descent-in-machine-learning)

And thats how we define our all coefficient ready to be suited in multivariable regression.
