---
title: Sample Resume with Math Showcase
layout: default
---

# John Doe's Resume

## Professional Summary
Experienced data scientist with a passion for machine learning and mathematical derivations. Skilled in Python, R, and statistical modeling. Seeking opportunities to apply analytic abilities in innovative projects.

## Education
- **M.S. in Data Science**, University of Example, 2023
- **B.S. in Mathematics**, College of Sample, 2021

## Experience
- **Data Analyst**, Tech Corp, 2023 - Present
  - Analyzed large datasets to drive business decisions.
  - Developed predictive models using regression techniques.
- **Research Assistant**, University Lab, 2021 - 2023
  - Conducted experiments on neural networks.
  - Published findings on optimization algorithms.

## Skills
- Programming: Python, R, SQL
- Tools: TensorFlow, Git, Jupyter
- Math: Linear Algebra, Calculus, Probability

## Certificates
- [Coursera Machine Learning](https://www.coursera.org/account/accomplishments/verify/EXAMPLE123) - [My Discussion & Derivations](/derivations/machine-learning-math)
- [Coursera Deep Learning Specialization](https://www.coursera.org/account/accomplishments/specialization/EXAMPLE456) - [My Analysis](/derivations/neural-net-derivations)

*This resume is designed to fit approximately one page when printed. For a PDF version, [download here](/assets/resume.pdf).*

---

# Sample Derivation Page (Linked from Certificates)

## Neural Network Backpropagation Derivation

Consider a simple feedforward neural network with one hidden layer. Let the input be \( \mathbf{x} \), hidden layer weights \( \mathbf{W}^{(1)} \), output weights \( \mathbf{W}^{(2)} \), and target output \( \mathbf{y} \).

The forward pass:
- Hidden activation: \( \mathbf{z} = \mathbf{W}^{(1)} \mathbf{x} \)
- Hidden output: \( \mathbf{h} = \sigma(\mathbf{z}) \) where \( \sigma \) is the sigmoid function: \( \sigma(z) = \frac{1}{1 + e^{-z}} \)
- Output: \( \hat{\mathbf{y}} = \mathbf{W}^{(2)} \mathbf{h} \)

The loss function (mean squared error): \( L = \frac{1}{2} \| \mathbf{y} - \hat{\mathbf{y}} \|^2 \)

Backpropagation gradients:

For output weights:
\[ \frac{\partial L}{\partial \mathbf{W}^{(2)}} = (\hat{\mathbf{y}} - \mathbf{y}) \mathbf{h}^T \]

For hidden weights:
\[ \delta = (\hat{\mathbf{y}} - \mathbf{y})^T \mathbf{W}^{(2)} \cdot \sigma'(\mathbf{z}) \]
\[ \frac{\partial L}{\partial \mathbf{W}^{(1)}} = \delta^T \mathbf{x} \]

Where \( \sigma'(z) = \sigma(z) (1 - \sigma(z)) \).

This derivation showcases the chain rule in action for gradient descent optimization.

For more details, explore advanced topics like vanishing gradients or alternative activations.