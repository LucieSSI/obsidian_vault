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

> [!example] **Notes (The "How")**
> ```neural network
> // Your code snippets here
> ```

---

## ⚠️ Debugging & Pitfalls
* **Common Error:** * **The Fix:** ---

## 🔗 Connections
- **Related Note:** [[ ]]
- **Official Docs:** [Link]
- **Back to Hub:** [[Neural Network MOC]]