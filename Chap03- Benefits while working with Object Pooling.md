## Benefits while working with Object Pooling

In the case of a shooter game, you can create and destroy bullets every single time or you can create a bunch beforehand and then reuse them like this:

- You spawn twenty or thirty bullets and put them in a pool.
- Whenever you fire your weapon, you a bullet from that pool.
- When the bullet hits something and disappears, you put it back into the pool.

This way, you save the CPU cycles it takes to instantiate and destroy these prefabs. Plus, you alleviate pressure on the garbage collector.
