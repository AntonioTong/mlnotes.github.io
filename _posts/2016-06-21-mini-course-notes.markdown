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
  wx+b=y
\end{align*}
$$

The output $y$ then passed through a softmax function $s(y)$: 

$$
\begin{align*}
  s(y_i) = \frac{e^{y_i}}{\sum_{j} e^{y_j}}
\end{align*}
$$

The softmax function will turn scores into probabilities. The identified class will have the highest probability, and the probability values of all classes add up to 1: $$\sum_{j}^{n} s(y_j) =1$$

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

