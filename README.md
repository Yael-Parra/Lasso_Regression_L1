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

(min over β)
   [ Σᵢ=1ⁿ (yᵢ − β₀ − Σⱼ=1ᵖ xᵢⱼ · βⱼ)² ] + λ · Σⱼ=1ᵖ |βⱼ|

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

| File Name           | Language | Description                                 |
|---------------------|----------|---------------------------------------------|
| `theory_english.md` | English  | Full explanation of Lasso Regression in English |
| `teoria_español.md` | Spanish  | Explicación completa de la Regresión Lasso en español |

---

## 🧑‍🏫 When to Use Lasso?

Use Lasso when you:
- Have **many features** and suspect some are irrelevant
- Want a **simpler, more interpretable model**
- Need to **prevent overfitting** in linear regression

---

## 🚀 Next Steps

- Explore the theory files for deeper understanding
- Try applying Lasso on real datasets (e.g., with scikit-learn)
- Experiment with different $\lambda$ values to see their effect on feature selection

---

## 🗣️ Multilingual Support

This project is designed to be **accessible to a wider audience**. All core explanations are available in both:
- <img src="https://upload.wikimedia.org/wikipedia/en/thumb/a/ae/Flag_of_the_United_Kingdom.svg/20px-Flag_of_the_United_Kingdom.svg.png" alt="Reino Unido" width="30" height="20">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; English:  
 **[theory_english.ipynb](theory_english.ipynb)** 
- <img src="https://upload.wikimedia.org/wikipedia/en/thumb/9/9a/Flag_of_Spain.svg/20px-Flag_of_Spain.svg.png" alt="España" width="30" height="20">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Spanish:   **[teoria_español.ipynb](teoria_español.ipynb)**

---

## 📬 Feedback

Have suggestions or questions? Feel free to open an issue or contribute!

