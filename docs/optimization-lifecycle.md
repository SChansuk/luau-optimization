The construction of an efficient software (or game, in this case) should be a continuous process. 
It is not a one-time task that you can complete and forget about. 

To begin with, the algorithms and data structures are designed in a way that makes sense for the application logic 
and that is reasonably efficient, but without considering optimization. 
When designing a widely used data structure the optimal implementation of which is not obvious 
(for example, it is debated whether it is better to use an array or a linked list), 
an abstract structure is defined for which the implementation may be changed at the optimization stage.
Secondly,  the code that implements the designed algorithms is written, following guidelines to avoid inefficient 
operations and encapsulating operations that are likely to require optimization.
Thirdly, The resulting software is then tested to increase the probability that it doesn't have crippling defects.
And lastly, After having completed the development of a correctly working application, the optimization stage begins,
with the following sub-stages: