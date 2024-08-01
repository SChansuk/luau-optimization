The construction of an efficient software, or rather game should adhere to the following development process:

**Design**: Firstly, the algorithms and data structures are designed in a way that makes sense for the application logic and that is reasonably efficient, but without considering optimization. 
When designing a widely used data structure where the optimal implementation is not obvious (for example, whether to use an array or a linked list), an abstract structure is defined for which the implementation may be changed at the optimization stage.

**Implementation**: Secondly, the code that implements the designed algorithms is written, following guidelines to avoid inefficient operations and encapsulating operations that are likely to require optimization.

**Functional Testing**: The resulting software is then tested to increase the probability that it doesn't have crippling defects.

**Optimization (aka Tuning)**: After having completed the development of a correctly working application, the optimization stage begins,
 with the following sub-stages:

1. Performance Testing: Commands with inadequate performance are detected. These are commands that, when processing typical data, require more resources (CPU time, storage space, etc.) than are available.
2. Profiling (aka Performance Analysis): For every command with inadequate performance, a profiler is used to determine which portions of code are the so-called bottlenecks for that command. Bottlenecks are parts of code where a disproportionate amount of time is spent or memory space is allocated.
3. Algorithmic Optimization: For each bottleneck, optimization techniques are applied that are largely independent of the programming language and totally independent of the platform. Such techniques can be found in algorithm theory textbooks. This optimization involves attempting to reduce the number of executed machine cycles. 
In particular, it involves reducing the number of calls to costly routines or transforming expensive operations into equivalent but less costly operations. For example, the quicksort sorting algorithm is chosen instead of the selection sort algorithm. If this makes the program fast enough, the optimization stage is complete.

This development process follows two criteria:

- Principle of Diminishing Returns: Optimizations that yield big results with little effort should be applied first, as this minimizes the time needed to reach the performance goals.
- Principle of Diminishing Portability: It is better to apply optimizations applicable to several platforms first, as they remain applicable on changing platforms and are more understandable to other programmers.

This stage sequence is not meant to be a one-way sequence, in which once one stage is reached, the preceding stage is no longer used. In fact, every stage may succeed or fail. If a stage succeeds, the next stage is applied, while if a stage fails, the previous stage is repeated, in a sort of backtracking algorithm.

In addition, a partial performance test should be performed after every optimization attempt, just to check whether the attempt was useful and, if so, to check whether more optimizations are needed.

Finally, after having completed the optimization, both the functional testing and the complete performance testing must be repeated to guarantee that the newly optimized version of the software is still functionally correct and has suitable performance.