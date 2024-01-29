Preference relation - weak

Two sets of goods (shopping carts) are comparable with the use of preference relation ≽ (not worse than).
The set of goods vectorX ≽ vectorY

Instead of choosing I prpose to introduce fuzzy logig with some functions wchich will signfy:

* OX: how prefered is vectorX (over some other goods)
* OY: [0,1] factor (normal fuzzy set functions).

> x = "oranges"
> y = "vegetables, water"
> z = "bread"

> variables <- set(preference = c(x=20, y=30, z=50), sd = 2)

Fuzzy rule may be which vector (shopping cart) is selected:

....... code

The example of fuzzy function is normal function with any standard deviation:

(img will be here from R)

The conditions:
* transitive
* connected

can be reflected in the fuzzy logic, on OX vector (shift).
> In R this is a *fuzzy partition*.

Various sets (shopping carts) which are fuzzy functions are tohether
> preference *field*
