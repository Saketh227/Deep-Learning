# Various Optimizers
```
    Gradient Descent
    Stochastic Gradient Descent (SGD)
    Mini Batch SGD
    SGD with momentum
    ADA Grad 
    ADA DELTA and RMS prop
    ADAM optimizer
```
# Epoch : 
# Iterarion :


---

# Gradient Descent Optimizer
![img_31.png](img_31.png)
![img_32.png](img_32.png)
![img_33.png](img_33.png)
```
Here in an epoch we send all data points at once and back propogate 
In the same way we continue till n epochs untill we minimize the cost function.

DisAdvantage:
    As we are processing all data points at once parallely we need machines with huge RAM and GPU.

So to avoid this requirement for intensive resources we get into SGD
```
---


# Stochastic Gradient Descent (SGD)
![img_34.png](img_34.png)
```
Here in an epoch during an iteration 1 data point is sent and back propogated.
Thus it performs multiple iterations in a single epoch till all the data points are sent and back propogated individually.

Multiple epochs are performed similarly till we get minimum Cost Function.

DisAdvantage:
    The Convergence will take time.
    Noise will get introduced ==> the movement seen in gradient descent graph above is noise.(no smooth convergence)
    
```



---
# Mini Batch Stochastic Gradient Descent
![img_35.png](img_35.png)
To Avoid disadvantages like resource intensive, slow convergence together we get into this.
```
Here we send data in a batch instead of sending individual or all at once.
In an epoch for a given iteration we send batch of records and for each iteration we send batches of data.
```
---

# SGD with Momentum
![img_36.png](img_36.png)
![img_37.png](img_37.png)
```
We have noise in above optimisers so we try to smoothen the weights to reduce noise.

We use Exponential weight Average 
```
![img_38.png](img_38.png)
```
We are trying to control a value based on previous value.
```

# ADA Grad (Adaptive Gradient descent)
![img_39.png](img_39.png)
```
We have a constant learning rate.
but to make convergence faster we can have dynamic learning rate which is high initially and low later.

Dis Advantage:
    There is possibility that alpha_t will be high making learning rate approx = 0
    which may lead to vanishing gradient
```

# ADA DELTA and RMS prop
![img_40.png](img_40.png)

# ADAM optimizer
![img_41.png](img_41.png)

