# **Gradient descent with google/jax**

Notebooks are executed on **Google Colab**.  
Original folder contains the original notebook, with jitted functions and plot, and is run with GPU.  
Benchmark folder contains the benchmark notebook, and device is specified in notebook's name.

## **Equation**
Equation used for this lab is:
$$
f(x) = 2x^{2} cos(x) -5x
$$

## **Benchmarks**

It's Intel Xeon(r) as CPU used for this benchmark (don't have more information from Google Colab), and Nvidia T4 as GPU.

|               | **Numpy/CPU** | **JAX/CPU** | **jit(JAX)/CPU** | **JAX/GPU** | **jit(JAX)/GPU** |
|:-------------:|:---------:|:-------:|:------------:|:-------:|:------------:|
|   **Total time**  |   173 µs  |  80 ms  |    14.4 µs   |  149 ms |    67.1 µs   |
| **Time per loop** |  57.1 µs  |  8.2 ms |    14.3 µs   | 59.5 ms |    27.5 µs   |
