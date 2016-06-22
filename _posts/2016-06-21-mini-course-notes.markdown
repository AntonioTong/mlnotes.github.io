---
layout: post
title:  "Deep Learning Notes"
date:   2016-06-21 16:17:57 -0700
categories: jekyll update
use_math: true
---

A linear classifier is presented by a simple logistic function with waights $w$ and bias $b$ parameters. 

$$
\begin{align*}
  wx+b=g
\end{align*}
$$

The output $y$ then obtained by pass the classifier through a softmax function $s(g)$: 

$$
\begin{align*}
  s(g_i) = \frac{e^{g_i}}{\sum_{j} e^{g_j}}
\end{align*}
$$

The softmax function will turn scores into probabilities. The identified class will have the highest probability, and the probability values of all classes add up to 1: $$\sum_{g}^{n} s(g_j) =1$$ .

Assume the estimated output is $$S=\left[0.7, 0.2, 0.1 \right]^T$$, and the actuall desired output is $$L=\left[1, 0, 0 \right]^T$$. A cross entropy function is defined:

$$
\begin{align*}
  D(S,L) = -\sum_{i} L_ilog(S_i)
\end{align*}
$$

To train such a linear classifier so that the waights $w$ and bias $b$ are properlly tuned to make correct classification given new data is to minimize the following Multinomial Logistic Classification function:

$$
\begin{align*}
  D(wx+b,L)
\end{align*}
$$

Hence we can define our cost function

$$
\begin{align*}
  \mathcal{L}=\frac{1}{N} \sum_{i} D(wx_i+b,L_i)
\end{align*}
$$
 

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

