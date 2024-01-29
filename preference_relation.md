Preference relation - weak

Two sets of goods (shopping carts) are comparable with the use of preference relation ≽ (not worse than).
The set of goods vectorX ≽ vectorY

Instead of choosing [x,y] I prpose to introduce fuzzy logic with some functions wchich will signfy:

* OX: how prefered is vectorX (over some other goods)
* OY: [0,1] factor (normal fuzzy set functions).

> x = "oranges"
> y = "vegetables, water"
> z = "bread"

> preference_rel = fuzzy_partition(varnames = c(vectorX = 20, vectorY = 30, vectorZ = 50), FUN = fuzzy_normal, sd = 2.0)

The example of fuzzy function is normal function with any standard deviation:

![image](https://github.com/jacekturek/fuzyecon/assets/62720909/505e0c4a-7087-4389-b7fd-56ea2d0db8a5)

The conditions:
* transitive
* connected

can be reflected in the fuzzy logic, on OX vector (shift).
> In R this is a *fuzzy partition*.

Various sets (shopping carts) which are fuzzy functions are tohether
> preference *field*
