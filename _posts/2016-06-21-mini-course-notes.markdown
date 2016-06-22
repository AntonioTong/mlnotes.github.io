---
layout: post
title:  "Deep Learning Notes"
date:   2016-06-21 16:17:57 -0700
categories: jekyll update
use_math: true
---

A linear classifier, 

$$
\begin{align*}
  wx+b=y
\end{align*}
$$

by waights $w$ and bias $b$, the output then passed through a soft max function $s(y)$ .

$$
\begin{align*}
  s(y_i) = \dfrac{e^(y_i)}}{\sum_{j} e^(y_j)}
\end{align*}
$$


Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

