# Preference relation - weak

Two sets of goods (shopping carts) are comparable with the use of preference relation ≽ (not worse than).
The set of goods vectorX ≽ vectorY

Instead of typical ranking [x,y] I prpose to introduce fuzzy logic with some functions wchich will signfy:

* OX: how prefered is vectorX (over some other goods)
* OY: [0,1] factor (normal fuzzy set functions).

> ⇨ x = "oranges"
> 
> ⇨ y = "vegetables, water"
> 
> ⇨ z = "bread"

> preference_rel = fuzzy_partition(varnames = c(vectorX = 20, vectorY = 30, vectorZ = 50), FUN = fuzzy_normal, sd = 2.0)

The example of fuzzy function is normal function with any standard deviation:

![image](https://github.com/jacekturek/fuzyecon/assets/62720909/505e0c4a-7087-4389-b7fd-56ea2d0db8a5)

The conditions for preference relation:
* 🎓 transitive
* 🎓 connected

can be reflected in the fuzzy logic, on OX vector (shift).
> ℹ️ In R this is a *fuzzy partition*.

Various goods vectors (shopping carts) which are fuzzy functions are tohether
> preference *field*

For the shopping carts where 
> x <= y AND x >= x

The relation is the indifference relation
which can mean that 

> there is no plot.

##

Similar plot and fuzzy set functions are for the 

> indiffernce relations

which is set of goods (fuzzy set) for the vectors (e.g. shopping carts) which are (all) equally good (*indifference relation*).

This set can be called an 

> indifference area (*for any goods vector x*).

##

Imagine several functions for shopping carts vectors x,y,z,..., wchich *together make a set M.* It will have a number of charts of functions like in the picture (each is a fuzzy function for one shopping cart).

>❗M-prefered cart is the best one (*most right function, calculated statistically*) - not shown - se above.
