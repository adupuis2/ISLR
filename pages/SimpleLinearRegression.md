# Simple Linear Regression  
Let **Y** be the true function of the sampled data.  
Let *y* be the estimated function of **Y**.  
Let *y*<sub>i</sub> = B<sub>0</sub> + B<sub>1</sub>*x*<sub>i</sub> be the prediction for **Y** based on the *i*th value of **X**.  
Then *e*<sub>i</sub> = (**Y**<sub>i</sub> - *y*<sub>i</sub>) − the difference between the actual **Y** value for x<sub>i and the predicted value at x<sub>i  
This error margin, or *residual*, for the *i*th sample is useful for determining the accuracy of a model.  
By taking the *residual* of all predictions where the associated sample value is available, it is possible to determine a number that roughly represents overall accuracy.

This is called the **Residual Sum of Squares (RSS)**.

**RSS** = (*e*<sub>1</sub>)<sup>2</sup> + (*e*<sub>2</sub>)<sup>2</sup> + (*e*<sub>3</sub>)<sup>2</sup> + ... + (*e*<sub>n</sub>)<sup>2</sup>

By utilizing this *least squares* approach, we are able to choose  B<sub>0</sub> and B<sub>1</sub> to minimize **RSS**.