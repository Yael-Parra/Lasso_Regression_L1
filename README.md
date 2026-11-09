# Lasso Regression L1  (Least Absolute Shrinkage and Selection Operator)

Welcome! This project provides a **clear and beginner-friendly explanation** of **Lasso Regression (L1 regularization)**, using intuitive examples and technical breakdowns — available in both **English and Spanish**.

---

## 📘 What is Lasso Regression?

**Lasso Regression** (Least Absolute Shrinkage and Selection Operator) is a type of **linear regression** that uses **L1 regularization**. Its main purposes are:

- 🔍 **Feature Selection**: It can automatically reduce some coefficients to **zero**, effectively removing less important features.
- 🧠 **Prevent Overfitting**: By simplifying the model, it helps improve generalization to new data.

---

## 🧮 The Cost Function

The Lasso cost function looks like this:

$$
\min_{\beta} \left\\{ \sum_{i=1}^{n} \Big(y_i - \beta_0 - \sum_{j=1}^{p} x_{ij}\beta_j\Big)^2 + \lambda \sum_{j=1}^{p} |\beta_j| \right\\}
$$

where $\lambda \ge 0$ controls the strength of the penalty (scikit-learn calls it `alpha`). The intercept $\beta_0$ is not penalized, and predictors should be standardized before fitting.

**Explanation**:

It minimizes the difference between actual and predicted values while penalizing the absolute magnitude of the coefficients to simplify the model and select important variables.

---

## ☕ Example: Coffee Shop Sales

Imagine you run a coffee shop and want to predict daily coffee sales based on:

- Weather (cold or hot)
- Weekend or weekday
- Whether there was a promotion
- If live music was playing
- And even quirky things like "Was the cat on the counter?"

Using Lasso, you can automatically discover which of these actually matter — and **ignore the noise**.

For example:
- The model may find that "cold weather" and "promotions" are strong predictors.
- But "the cat being on the counter"? 👀 Likely gets a coefficient of **zero**, meaning it's irrelevant.

---

## 📁 Files Included

| File | Language | Description |
|------|----------|-------------|
| [`theory_english.ipynb`](theory_english.ipynb) | English | Full explanation of Lasso Regression |
| [`teoria_español.ipynb`](teoria_español.ipynb) | Spanish | Explicación completa de la Regresión Lasso |
| [`teoria_español.pdf`](teoria_español.pdf) | Spanish | PDF export of the Spanish theory notebook |
| [`ejemplo_lasso.ipynb`](ejemplo_lasso.ipynb) | Spanish | Practical example with scikit-learn `LassoCV` on the `tips` dataset |

---

## 🧑‍🏫 When to Use Lasso?

Use Lasso when you:
- Have **many features** and suspect some are irrelevant
- Want a **simpler, more interpretable model**
- Need to **prevent overfitting** in linear regression

---

## 🚀 Next Steps

- Explore the theory files for deeper understanding
- Run the practical example [`ejemplo_lasso.ipynb`](ejemplo_lasso.ipynb) (`pip install -r requirements.txt`)
- Try applying Lasso on real datasets (e.g., with scikit-learn)
- Experiment with different $\lambda$ values to see their effect on feature selection

---

## 🗣️ Multilingual Support

This project is designed to be **accessible to a wider audience**. All core explanations are available in both:

- <span style="display:inline-block; width: 35px;"><img src="https://upload.wikimedia.org/wikipedia/en/thumb/a/ae/Flag_of_the_United_Kingdom.svg/20px-Flag_of_the_United_Kingdom.svg.png" alt="UK" width="30" height="20"></span> English: [theory_english.ipynb](theory_english.ipynb)
- <span style="display:inline-block; width: 35px;"><img src="https://upload.wikimedia.org/wikipedia/en/thumb/9/9a/Flag_of_Spain.svg/20px-Flag_of_Spain.svg.png" alt="Spain" width="30" height="20"></span> Spanish: [teoria_español.ipynb](teoria_español.ipynb)


---

## 📬 Feedback

Have suggestions or questions? Feel free to open an issue or contribute!

