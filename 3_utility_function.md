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

What is importnant in utility functions (apart from analytical formula) it is Hessian (second derivatives matrix over the goods). Question here is can we model in AI the Hessian >= 0? I think we can consider Hessian in the fuzzy set function (p=>q) and state it's > 0 for one factor. It can be done by the definiotion of the transformation FI(x) -> y.
