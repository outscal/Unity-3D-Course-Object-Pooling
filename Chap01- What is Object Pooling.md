## **What is Object Pooling?**

Object pooling is a software creational design pattern and a container of objects that holds a list of other objects—those are ready to be used. Once an object is taken from the pool, it is not available in the pool until it is put back. Object pooling keeps track of Objects—those are currently in use, the number of objects the pool holds, and whether this number should be increased. Objects in the pool have a lifecycle of creation, validation, and destruction.

Instantiate() and Destroy() are useful and necessary methods during gameplay. Each generally requires minimal CPU time.

However, for objects created during gameplay that have a short lifespan and get destroyed in vast numbers per second, the CPU needs to allocate considerably more time.

**Bullets are a great example of a GameObject that you might pool.**

Additionally, Unity uses Garbage Collection to deallocate memory that’s no longer in use. Repeated calls to Destroy() frequently trigger this task, and it has a knack for slowing down CPUs and introducing pauses to gameplay.

This behaviour is critical in resource-constrained environments such as mobile devices and web builds.


