# Simple Linear Regression  
Let **Y** be the true function of the sampled data.  
Let *y* be the estimated function of **Y**.  
Let <pre>*y*<sub>i</sub> = B<sub>0</sub> + B<sub>1</sub>*x*<sub>i</sub></pre> be the prediction for **Y** based on the *i*th value of **X**.  
Then <pre>*e*<sub>i</sub> = (**Y**<sub>i</sub> - *y*<sub>i</sub>)</pre> is the difference between the actual **Y** value for x<sub>i</sub> and the predicted value at x<sub>i</sub>  
This error margin, or *residual*, for the *i*th sample is useful for determining the accuracy of a model.  
By summing the *residual* of all predictions where the associated sample value is available, it is possible to derive a number that roughly represents overall accuracy. In simpler terms: it is the combined error margin for all x<sub>i</sub> and the smaller you can get it, the more accurate the model is overall.

This is called the **Residual Sum of Squares (RSS)**.

<pre>**RSS** = (*e*<sub>1</sub>)<sup>2</sup> + (*e*<sub>2</sub>)<sup>2</sup> + (*e*<sub>3</sub>)<sup>2</sup> + ... + (*e*<sub>n</sub>)<sup>2</sup></pre>

By utilizing this *least squares* approach, we are able to choose  B<sub>0</sub> and B<sub>1</sub> to minimize **RSS**. The *minimizers* are...

<pre>B<sub>1</sub> = sum([x<sub>i</sub> - mean(x)][y<sub>i</sub> - mean(y)])
    = the sum of (x residuals times y residuals)
    
B<sub>0</sub> = mean(y) - B<sub>1</sub>mean(x)
    = (the mean of y) minus (B<sub>1</sub> times the mean of x)
</pre>