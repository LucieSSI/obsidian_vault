---
type: ml-note
subject: "[[Neural Network MOC]]"
language: Neural Network
status: 🌱 Learning
date: 2026-03-05
---
# 📝 Topic: Neurons & Functions

> [!abstract] **Logic Summary**
> *Neurons are stackable units that take inputs, and produce a singular output. Using the sigmoid function as its activation.*

---

## 💡 Concepts & Code

> [!question] **How do Neurons work?**
> **Definition:** Neurons take inputs $x$, utilizes an activation function (Sigmoid Function) $\frac{1}{1+e^{-x}}$ to produced a value that limits all $-\infty$ as 0, and $+\infty$ as 1.
> 
> **What Neurons do::** 
> Start with multiplying each input by $w$ or weight
> $$x_1 \rightarrow x_1 * w_1$$ $$x_2 \rightarrow x_2 * w_2$$
> Next, all weighted values are summarized with a $b$ or bias
> $$(x_1 * w_1) + (x_2 * w_2) + b = z$$
> Now it's substituted into our activation function
> $$\frac{1}{1+e^{-z}}$$

> [!example] **Neurons in Python**
> ```python
> # For this project, Numpy's heavily utilized, and allows the neurons to function.
> import numpy as np
> 
> def sigmoid(x):
> 	# Define our activation function 
> 	return 1 / (1 + np.exp(-x))
> 
> # Now to create the actual Neurons
> class Neuron:
> 	def __init__(self, weight, bias):
> 		self.weights = weight
> 		self.bias = bias
> 	
> 	def feedforward(self, inputs):
> 		total = np.dot(self.weights, inputs) + self.bias
> 		return sigmoid(total)
> weights = np.array([0,1])
> bias = 4
> n = Neuron(weights, bias)
> 
> x = np.array([-1,-2])
> print(n.feedforward(x))
> ```

---

## ⚠️ Debugging & Pitfalls
* **Common Error:** * **The Fix:** ---

## 🔗 Connections
- **Related Note:** [[ ]]
- **Official Docs:** [Link]
- **Back to Hub:** [[Neural Network MOC]]