# Flo
Flo is a Domain-Specific Language (DSL) for High-Performance Computing that uses fluid dynamics metaphors to enforce Memory Locality and Cache-Aware programming

In modern hardware, the bottleneck is rarely the CPU. It’s the Memory Wall. Flo performs Static Analysis on data access patterns to categorize them. Sequential, cache-friendly access is treated as Laminar, while high-stride or random access is flagged as Turbulent. By assigning 'Mass' and 'Momentum' to data objects based on their access frequency and size, the compiler can automatically suggest or implement Tiling and Vectorization strategies to minimize latency.
