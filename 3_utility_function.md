In short mathematically related function U with preference relation is called utility function. 
Without formulas you can describe the utility function as continuoes as the relation of preference is continuous.
In R^n+ which is the space of goods. 

> #cone is one of the possible functions
> 
> utility <- fuzzy_cone(center = NULL, radius = 1, height = 1, return_base_corners=TRUE)
>
> plot(utility)

Here is my AI simulation, with fuzzy sets of a cotnunuous utiility function:

![image](https://github.com/user-attachments/assets/8329e4a9-a149-4b1e-9815-71be10f85803)

📌 Here I can suppose there is no shortage in goods (fenomenon) because it would imply that for a greater vector of goods Vx > Vy there is a strong (≻) preference for Vx. This is not possible in the chart.

📌 Utility functions by definition which are convex are important in economics. I can model this with sets lib - excluding the subset of statistically non-convex functions - here the data:

> .N.(c(2,2,1))
> 
> [1] -1 -1  0

📉 For cars (if we have a look on a market) let us prove the I Law Gossen about margin utility:

> .I.(c(2,2,4),c(2,2,1)) [^1]
>
> [1] 1 1 1

It doesn't work in this example.

[^1]: Here the funcion .I. means fuzzy implication (similar to the .N. - fuzzy negation).
