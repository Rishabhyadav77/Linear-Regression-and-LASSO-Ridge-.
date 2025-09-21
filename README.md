Linear Regression

Linear regression is like drawing the best possible straight line (or plane) through the data so we can predict outcomes.
Equation looks like:

𝑦
=
𝛽
0
+
𝛽
1
𝑥
1
+
𝛽
2
𝑥
2
+
.
.
.
+
𝛽
𝑛
𝑥
𝑛
+
𝜖
y=β
0
	​

+β
1
	​

x
1
	​

+β
2
	​

x
2
	​

+...+β
n
	​

x
n
	​

+ϵ

𝑦
y → the value we want to predict

𝑥
x’s → features (inputs)

𝛽
β’s → weights/coefficients (how important each feature is)

𝜖
ϵ → error

The goal is to minimize the error (difference between predicted and actual).

👉 Works well for simple data, but… if features are correlated or there are too many, it can overfit.

🔹 Regularization – Fix for Overfitting

Regularization = adding a penalty to the model so it doesn’t rely too heavily on certain features.

Two main types:

1. Ridge Regression (L2 Regularization)

Adds a penalty based on the square of coefficients.

It makes coefficients smaller but never exactly zero.

Good when all features are somewhat useful.

Think of it like: “Keep everything, but control the weight.”

Equation:

𝐿
𝑜
𝑠
𝑠
=
𝑀
𝑆
𝐸
+
𝜆
∑
𝛽
𝑗
2
Loss=MSE+λ∑β
j
2
	​

2. Lasso Regression (L1 Regularization)

Adds a penalty based on the absolute value of coefficients.

Pushes some coefficients all the way to zero → automatic feature selection.

Best when you have many features and only some really matter.

Equation:

𝐿
𝑜
𝑠
𝑠
=
𝑀
𝑆
𝐸
+
𝜆
∑
∣
𝛽
𝑗
∣
Loss=MSE+λ∑∣β
j
	​

∣
