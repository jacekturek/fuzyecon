# Budget field

Assume the consumer has a budget i.e. amount of money she can spend

> ❗ the 'shopping cart' VectorX

> ❗the prices of each unit in VectorX namely VectorP

The scalar multiplication:

> VectorX ⊕ VecorP <= I

where

> I - budget limit

The set of 'shopping carts' like all Vectors for which the <= conditon is true
is not a fuzzy set of cours but the set is important in math. economics and called

> budget

The set where the VectorX ⊕ VecorY = I (rather than <=), is called the budget field.

The fuzzy sets can be a research tool also for the budget:

*budget = fuzzy_partition(varnames = c(budg1 = 3, budg2 = 4), FUN = fuzzy_normal, sd = 3.0)*

> a fuzzy partition shows budget fields:

![image](https://github.com/jacekturek/fuzyecon/assets/62720909/c45da371-3361-4be9-8f79-ef3141fbd09a)

The *Z(VecP,I)-optimal* shopping cart is a Vector within the budget
> for which any other cart is worse (perf. rel is in other part).
