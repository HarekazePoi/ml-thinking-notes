# Bias vs Variance (My Understanding)

At first, I treated bias and variance as definitions to memorize.
I only truly understood them after seeing how different models fail in practice.

## What bias means to me

High bias means the model is **too simple**.
It makes strong assumptions and cannot capture the underlying pattern well.

Typical signs:
- Underfitting
- High training error
- High validation error

## What variance means to me

High variance means the model is **too sensitive to the training data**.
It fits noise instead of the true pattern.

Typical signs:
- Very low training error
- Much higher validation/test error

## The trade-off

I now think of the bias–variance trade-off as a balance problem:

- Simpler model → higher bias, lower variance
- More complex model → lower bias, higher variance

The goal is not to minimize one, but to find a good balance.

## A mistake I made before

I used to believe:
> "More complex models are always better."

Now I know that without enough data or regularization,
complex models can easily overfit.
