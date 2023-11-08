# Quantum-inspired-algorithms
 Quantum-inspired algorithms for Portfolio optimization

## Dataset: S & P-500 stock index
## Model: Markowitz Mean-Variance model

## Quadratic Program:
$$minimize\ (over\ w): w^T\Sigma w$$

$$ such\ that\ : r^T w = \mu $$

$$ where \ \Sigma \rightarrow correlation\ matrix;\ r\rightarrow expected\ return; \mu \rightarrow target\ return $$

## Using KKT condition for constrained optimization to convert it into a linear system of equations:

$$ \Sigma w + r^T\lambda =0 $$

$$ r^T w = \mu $$

$$ where \ \lambda \rightarrow Lagrange\ multiplier $$

## We solve it in two ways:
> Quantum-inspired algorithm (QIA): a sampling-based technique to approximate solution; runtime polylogarithmic in problem size
>
> Direct classical method DCM(): Analytical solution; runtime is linear in problem size
>

## Result: 
> For small and moderate-sized problems, DCM is beneficial.
>
> For relatively large problem size, QIA outperform DCM after a certain value 'n'.
