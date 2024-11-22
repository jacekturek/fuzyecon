# Preference relation - weak

Two sets of goods (shopping carts) are comparable with the use of preference relation ≽ (not worse than).
The set of goods vectorX ≽ vectorY

Instead of typical ranking [x,y] I prpose to introduce fuzzy logic with some functions wchich will signfy:

* OX: how much a shopping car is prefered (over some other goods)
* OY: [0,1] fuzzy function value (normal fuzzy set functions).

> Fuzzy set function (element f(element)) - f: how much an element belongs to a set

This is called fuzzy functions.

Let's look at three 'shopping carts':

> ⇨ x = "oranges"
> 
> ⇨ y = "vegetables, water"
> 
> ⇨ z = "bread"

 or in terms of data categorization:

> shoppingcart <- factor(c("oranges","vegetables,water","bread"))
> 
> shoppingcart
> 
> [1] oranges          vegetables,water bread
>         
> Levels: bread oranges vegetables,water

normally, without fuzzy logic:

> shoppingcart <- data.frame(cart=factor(c("oranges","vegetables,water","bread")))
>
> shoppingcart$ranking <- c(0,1,1)

> shoppingcart

> cart ranking
> 
> 1          oranges       0
> 
> 2 vegetables,water       1
> 
> 3            bread       1
> 

now, the fuzzy sets can help:

> 📝 preference_rel = fuzzy_partition(varnames = c(vectorX = 20, vectorY = 30, vectorZ = 50), FUN = fuzzy_normal, sd = 2.0)

The example of fuzzy function is normal function with any standard deviation:

![image](https://github.com/jacekturek/fuzyecon/assets/62720909/505e0c4a-7087-4389-b7fd-56ea2d0db8a5)

##

Only to think : the conditions for preference relation:
* 🎓 transitive pRq and qRr => pRr
* 🎓 connected pRr or rRp

can be reflected in the fuzzy logic, on OX vector (shift).
> ℹ️ In R this is a *fuzzy partition*.

##

Various goods vectors (shopping carts) which are fuzzy functions are tohether
> preference *field*

For the shopping carts where 
> x <= y AND x >= x

The relation is the indifference relation
which can mean that 
> there is no plot - assumedly.

Virtually there are many carts, sometimes there is no difference in which I choose.

##

> Other than fuzzy parition is fuzzy rules, I will not introduce it now but fuzzy rule can be someting like:
> if vector of goods = x and not y and not x => choose x because no better one is avaiable.

> 🎓 (this is to explain the relation of preference).

##

Similar plot and fuzzy set functions are for the 

> indiffernce relations

which is set of goods (fuzzy set) for the vectors (e.g. shopping carts) which are (all) equally good (*indifference relation*).

This set can be called an 

> indifference area (*for any goods vector x*).

Statistically I add some fuzzy LOGIC like negation:

> .N.(c(1,1,2,6)) # ✅ fuzzy negation

> [1]  0  0 -1 -5

for the previous data.

##

Imagine several functions for shopping carts vectors x,y,z,..., wchich *together make a set M.* This is as well a set of fuzzy set functions like in the picture (each is a fuzzy function for one shopping cart).

>❗M-prefered cart is the best one (*most right function, calculated statistically*) - not shown - se above.

TO be more creative in modeling ✔️, as models are contepoarary stories about economics, I want again fuzzy_parition for M-preferred chart of goods:

> m_pref = fuzzy_partition(varnames = c(x = 1 , y=2, z=1), FUN = fuzzy_cone, radius = 8)

![image](https://github.com/user-attachments/assets/058eba74-c306-4cd7-9a1b-bf7900a83f2d)

