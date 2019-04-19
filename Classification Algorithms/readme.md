# Classification Algorithm

The following programs are used for classification algorithms such as Decision Trees.

## Info

Used in Gain calculation, Gain is defined as follows:

```math
Gain(A)=Info(D)−Info_A (D)
```

Info is

```math
Info(D)=-\sum_{i=1}^{m}p_i\log_2(p_i)
```

and $`p_i`$ is

```math
p_i = \frac{\left | C_i,_D \right |}{\left | D \right |}
```

e.g.:

```
Info(5,3)=-\frac{5}{8}\log_2\left (\frac{5}{8}  \right )-\frac{3}{8}\log_2\left (\frac{3}{8}  \right )
```
