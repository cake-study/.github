# Cake Study

"Cake Study" shows how to integrate automated tests in different languages in frameworks with the
[Qase TMS](https://qase.io).

All test examples use the same story: making a cake. There is an implementation of the Cake class and tests that check it's behavior.

Making a cake takes several steps:

1. Get some uncooked ingredients for a new cake. 
1. Shake them well to make a raw cake.
1. Bake the cake. Now it's ready! 
1. Take the cake home.


```
Shake it, bake it, take it, taste it;
Our cakes are never over.
```

## Detailed requirements

Implementation and testing require a detailed description of states of a Cake object and transitions between them.

A cake has the following states: 

*   Uncooked (initial state)
*   Raw (after shaking)
*   Baked (after baking)
*   Taken (after being taken home)
*   Burned (error state after baking too much)

There are the following transitions between states:

* Constructor should create an "uncooked" cake. 
*  `shake()` changes an "uncooked" cake to "raw". Has no effect on a "raw", "baked", or "taken" cake.
* `bake()` makes "raw" cake "baked". Baking an already "baked" cake should make it "burned".
* `take()` turns a "baked" cake into "taken".


There should be a special method or property for checking the state of a Cake: `cake.state()` or `cake.state`.


