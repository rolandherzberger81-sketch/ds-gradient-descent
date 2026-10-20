# Gradient Descent

The goal of almost any machine learning model is to find the parameters that minimize a cost function. Gradient descent is the workhorse method for doing that. This repo takes gradient descent apart at a granular level: you read code that performs each step, see what the optimization looks like visually, write the algorithm yourself from scratch, and finish with a small classification example. Linear regression is the running example, but the method is the same one used to train far larger models.

## Learning Objectives

By the end of this repository, you should be able to:

- Explain what a cost function is and why minimizing it is the goal of training.
- Derive the gradient of a simple cost function and use it to update parameters.
- Distinguish batch, stochastic, and mini-batch gradient descent and when each is used.
- Describe how momentum changes the path gradient descent takes.
- Implement gradient descent from scratch in Python.
- Apply gradient-descent-based learning to a classification problem with `SGDClassifier`.

## Learning Path

Work through the notebooks in order; each one builds on the previous.


| File / Folder | Description |
|---|---|
| [**1 - Gradient Descent**](1_gradient_descent.ipynb) | Cost functions and gradients, with batch, stochastic, and mini-batch gradient descent on a linear regression. |
| [**2 - Gradient Descent Visualization**](2_gradient_descent_visualization.ipynb) | What the optimization path looks like, and how momentum changes it. |
| [**3 - Gradient Descent Codealong**](3_gradient_descent_codealong.ipynb) | Write your own gradient descent from scratch, step by step. |
| [**4 - Bonus: Classification**](4_bonus_classification.ipynb) | A classification example using `SGDClassifier` to preview supervised learning. |

### Additional Folders and Files

| File / Folder | Description |
|---|---|
| [**Assets**](assets/) | Animations used in the visualization notebook. |
| [**Solutions**](solutions/) | Reference solutions. |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies. |
| [**uv.lock**](uv.lock) | Dependency lock file. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a **placeholder**. Replace it, including the `< >` brackets, with your own value. For example, `cd <repo-name>` becomes `cd ds-gradient-descent`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like `git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in `.venv/`.

```bash
cd <repo-name>
uv sync
```

---

### 5. Open the Notebooks

> [!NOTE]
> Make sure you open VS Code from the project root so it automatically detects the environment created by `uv sync`.

Launch VS Code in the project root folder:

```bash
code .
```

Then open a notebook and select the Python environment created by `uv sync` as the kernel.

## How to use this repo

Work through the notebooks in the order listed above. In the first notebook, read the code that performs each step of gradient descent and document what happens in each line. The second notebook shows you what gradient descent looks like visually. In the third, it is your job to write gradient descent from scratch. The last notebook is a short classification example that previews what comes next.

## References & Further Reading

- [**An overview of gradient descent optimization algorithms**](https://www.ruder.io/optimizing-gradient-descent/): A widely cited tour of batch, stochastic, and mini-batch gradient descent and the optimizers built on them.
- [**Why Momentum Really Works (Distill)**](https://distill.pub/2017/momentum/): An interactive explanation of how momentum speeds up gradient descent.
- [**Stochastic Gradient Descent (scikit-learn)**](https://scikit-learn.org/stable/modules/sgd.html): The reference for `SGDClassifier` and `SGDRegressor` used in the bonus notebook.
- [**Multiplying Matrices**](https://www.mathsisfun.com/algebra/matrix-multiplying.html): A refresher on the matrix math behind the vectorized gradient computations.
