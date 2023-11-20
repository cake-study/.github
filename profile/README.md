# Cake Study

"Cake Study" shows how to integrate automated tests in different languages in frameworks with the
[Qase TMS](https://qase.io).

## Making Cakes

All tests examples use the same object: a cake.

*   `shake()`: Transitions an "uncooked" cake to "raw". Has no effect on a "raw", "baked", or "taken" cake. Throws a special message and an exception for a "burned" cake.
*   `bake()`: Transitions a "raw" cake to "baked". Transitions a "baked" cake to "burned" (error state). Throws an exception if attempted on an "uncooked" or "burned" cake.
*   `take()`: Transitions a "baked" cake to "taken". Throws an exception if attempted on cakes in any other state.
*   `state()`: Returns the current state of the cake.


A cake has the following states:
*   Uncooked (initial state)
*   Raw (after shaking)
*   Baked (after baking)
*   Taken (after being taken home)
*   Burned (error state after double baking)
