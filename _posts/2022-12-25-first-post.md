---
title: "First post"
layout: post
mathjax: true
---

Hello! This is my first test post on my blog. Hopefully I'll add more here later!

In the meantime, here is the equation for the forward diffusion process:

$$ \mathbf{x}_t = \sqrt{\bar{\alpha}_t} \mathbf{x}_0 + \sqrt{1 - \bar{\alpha}_t} \epsilon, \ \ \epsilon \sim \mathcal{N}(\mathbf{0}, \mathbf{I}), $$

along with some code:

{% highlight python %}
beta = np.array(noise_schedule)
noise_level = np.cumprod(1 - beta)
noise_level = torch.tensor(noise_level.astype(np.float32))
{% endhighlight %}

Here is also some Go code:

{% highlight go %}
func (a *value) Mul(b *value) *value {
    out := Value(a.Val * b.Val)
	out._op = "*"
	out._prev[a], out._prev[b] = true, true
	
	// In the case of c = a * b, c will here be 'out'
	// so we need to make sure it's gradient is set to 1 in '_backward'
	out._backward = func (out *value) () {
		a.Grad += b.Val * out.Grad
		b.Grad += a.Val * out.Grad
	}

	return out
}
{% endhighlight %}