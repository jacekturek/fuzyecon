# Budget field

Assume the consumer has a budget i.e. amount of money:

> ❗ the 'shopping cart' VectorX

> ❗the prices of each unit in VectorX namely VectorP

> VectorX ⊕ VecorP <= I

where

> I = budget limit
> ⊕ - scalar multiplication

The set of 'shopping carts' for which ... ⊕ ... <= I are called to be possible for consumer:

> these "shopping carts" are => within the budget

> #vegetables, bread+water, oranges
> 
> A <- gset(letters[1:3], memberships = c(1,3,2)) [^1]
> 
> plot(A)

![image](https://github.com/user-attachments/assets/8a17cf9c-ea16-4bae-b38c-e37a89e73f70)


The set where the VectorX ⊕ VecorY = I (rather than <=), is called *budget field*.

The fuzzy sets are good for showing budgets:

*budget = fuzzy_partition(varnames = c(budg1 = 3, budg2 = 4), FUN = fuzzy_normal, sd = 3.0)*

> some fuzzy partition shows budget fields:

![image](https://github.com/jacekturek/fuzyecon/assets/62720909/c45da371-3361-4be9-8f79-ef3141fbd09a)

The *Z(Vp,I)-optimal* shopping cart is a Vector within the budget
> for which any other cart is worse (perf. rel is in other part).

Can looking for the Z(p,I) prefered shopping cart be modeled with fuzzy negation?
Here's a model:

> charts_budg_field <- c(2,2,8)
> 
> .N.(charts_budg_field) [^2]
> 
> [1] -1 -1 -7

[^1]: gset is a generlized set (element, membership function)
[^2]: fuzzy negation
