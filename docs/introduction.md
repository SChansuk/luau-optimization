# Introduction to Optimization

One of the main reasons for preferring Luau over simpler, higher-level scripting languages is that Luau allows for the 
development of complex Roblox games with an efficient use of hardware resources. The language itself doesn't guarantee 
efficient code automatically, but it provides a robust set of features that aid developers in achieving performance gains. 

Sloppy Luau code may be no more efficient than higher-level implementations of the same algorithms, 
but a skilled Luau programmer with in-depth knowledge of the language can write software that is efficient 
from the start and further optimize it as needed. 

This guide offers techniques for writing efficient Luau code and optimizing existing game scripts. 
Often, there is no single solution to a performance problem that is optimal for all scenarios.
 Therefore, optimization typically involves incrementally refactoring code to improve performance, 
 bringing it closer to the best possible outcome.

Effective optimization requires that the codebase is modular enough to isolate performance-critical sections. 
With well-structured code, you can then use various tools, libraries, and strategies to enhance these parts, 
thereby boosting the overall execution speed of your game. While modern game engines and platforms 
like Roblox perform many optimizations automatically, there are still higher-level optimizations that developers must address. 
This guide focuses on those optimizations that current engines and compilers cannot (yet) achieve.

Most of the optimization techniques discussed are platform-independent, so there will be minimal references to specific operating systems, hardware, or Roblox Studio versions. However, some techniques might be more effective or applicable depending on the specific combinations of platform, hardware, and version of Roblox Studio you are using.