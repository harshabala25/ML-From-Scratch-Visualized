# ML From Scratch, Visualized

Hand-coded implementations of core algorithms from Andrew Ng's Machine Learning
Specialization (Stanford / DeepLearning.AI), built from scratch using NumPy to
develop a real understanding of the math before relying on libraries like
scikit-learn — paired with a full-stack web app that visualizes each algorithm
training in real time (loss curves, decision boundaries, moving cluster
centers, etc.).

## Why this project exists

Most "ML from scratch" repos are a folder of scripts you have to read to
appreciate. This one lets you actually watch the algorithms learn — pick a
model, feed it data, and see gradient descent converge, a decision boundary
shift, or clusters form step by step, all powered by hand-written NumPy code
underneath (no sklearn/PyTorch doing the heavy lifting).

## Planned algorithms (following the course sequence)

**Course 1 — Supervised Learning: Regression & Classification**
- [ ] Linear regression (gradient descent, cost function, feature scaling)
- [ ] Logistic regression (decision boundary, regularization)

**Course 2 — Advanced Learning Algorithms**
- [ ] Neural network (forward propagation + backpropagation from scratch)
- [ ] Decision tree

**Course 3 — Unsupervised Learning, Recommenders, RL**
- [ ] K-means clustering
- [ ] Simple collaborative-filtering recommender

## Stack

- **Backend:** Python, NumPy (core algorithm implementations), FastAPI (serving
  training runs/predictions to the frontend)
- **Frontend:** React (interactive visualizations of training in progress)
- **Testing:** Each implementation is validated against scikit-learn's
  equivalent to confirm correctness

## Project structure

```
backend/
  algorithms/       # hand-coded NumPy implementations, one file per algorithm
  tests/            # correctness tests, validated against sklearn
  api/              # FastAPI endpoints exposing training runs to the frontend
frontend/
  src/              # React app — algorithm picker + live visualizations
notebooks/          # scratch work / exploration while learning each concept
```

## Status

Actively in progress — building this alongside working through the course
material, roughly one algorithm at a time.

## Background

Built while working through Andrew Ng's Machine Learning Specialization to
reinforce the math with a working implementation, and to make the concepts
demoable rather than just readable.
