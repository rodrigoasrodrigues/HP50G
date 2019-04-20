# Classification Algorithm

The following programs are used for classification algorithms such as Decision Trees.

## Info

Used in Gain calculation, Gain is defined as follows:

![Gain(A)=Info(D)-Info_A(D)](https://latex.codecogs.com/gif.latex?Gain%28A%29%3DInfo%28D%29-Info_A%28D%29)

Info is

![Info(D)=-\sum_{i=1}^{m}p_i\log_2(p_i)](https://latex.codecogs.com/gif.latex?Info%28D%29%3D-%5Csum_%7Bi%3D1%7D%5E%7Bm%7Dp_i%5Clog_2%28p_i%29)

and ![p_i](https://latex.codecogs.com/gif.latex?p_i) is

![p_i = \frac{\left | C_i,_D \right |}{\left | D \right |}](https://latex.codecogs.com/gif.latex?p_i%20%3D%20%5Cfrac%7B%5Cleft%20%7C%20C_i%2C_D%20%5Cright%20%7C%7D%7B%5Cleft%20%7C%20D%20%5Cright%20%7C%7D)

e.g.:

![Info(5,3)=-\frac{5}{8}\log_2\left (\frac{5}{8}  \right )-\frac{3}{8}\log_2\left (\frac{3}{8}  \right )](https://latex.codecogs.com/gif.latex?Info%285%2C3%29%3D-%5Cfrac%7B5%7D%7B8%7D%5Clog_2%5Cleft%20%28%5Cfrac%7B5%7D%7B8%7D%20%5Cright%20%29-%5Cfrac%7B3%7D%7B8%7D%5Clog_2%5Cleft%20%28%5Cfrac%7B3%7D%7B8%7D%20%5Cright%20%29)

## Gini

Calculates the Gini Index given two values