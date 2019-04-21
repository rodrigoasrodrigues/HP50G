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

## SplitInfo

Using in GainRatio Calculation:

![GainRaio(A) = \frac{Gain(A)}{SplitInfo(A)}](https://latex.codecogs.com/gif.latex?GainRaio%28A%29%20%3D%20%5Cfrac%7BGain%28A%29%7D%7BSplitInfo%28A%29%7D)

The formula is:

![SplitInfo_A(D)=-\sum_{j=1}^{v}\frac{\left | D_j \right |}{\left | D \right |}\times \log_2\left ( \frac{\left | D_j \right |}{\left | D \right |} \right )](https://latex.codecogs.com/gif.latex?SplitInfo_A%28D%29%3D-%5Csum_%7Bj%3D1%7D%5E%7Bv%7D%5Cfrac%7B%5Cleft%20%7C%20D_j%20%5Cright%20%7C%7D%7B%5Cleft%20%7C%20D%20%5Cright%20%7C%7D%5Ctimes%20%5Clog_2%5Cleft%20%28%20%5Cfrac%7B%5Cleft%20%7C%20D_j%20%5Cright%20%7C%7D%7B%5Cleft%20%7C%20D%20%5Cright%20%7C%7D%20%5Cright%20%29)

e.g.:

![SplitInfo({4,6,4})=-\frac{4}{14}\log_2 \frac{4}{14}-\frac{6}{14}\log_2 \frac{6}{14}-\frac{4}{14}\log_2 \frac{4}{14} = 1.557](https://latex.codecogs.com/gif.latex?SplitInfo%28%7B4%2C6%2C4%7D%29%3D-%5Cfrac%7B4%7D%7B14%7D%5Clog_2%20%5Cfrac%7B4%7D%7B14%7D-%5Cfrac%7B6%7D%7B14%7D%5Clog_2%20%5Cfrac%7B6%7D%7B14%7D-%5Cfrac%7B4%7D%7B14%7D%5Clog_2%20%5Cfrac%7B4%7D%7B14%7D%20%3D%201.557)

## Gini Index

Calculates the Gini Index given a List of Values:

![gini(D)=1-\sum_{j=1}^{n} p_j^2](https://latex.codecogs.com/gif.latex?gini%28D%29%3D1-%5Csum_%7Bj%3D1%7D%5E%7Bn%7D%20p_j%5E2)

E.g.:

![gini(\{9,5\})= 1 - \left ( \frac{9}{14} \right )^2-\left ( \frac{5}{14} \right )^2 = 0.459](https://latex.codecogs.com/gif.latex?gini%28%5C%7B9%2C5%5C%7D%29%3D%201%20-%20%5Cleft%20%28%20%5Cfrac%7B9%7D%7B14%7D%20%5Cright%20%29%5E2-%5Cleft%20%28%20%5Cfrac%7B5%7D%7B14%7D%20%5Cright%20%29%5E2%20%3D%200.459)