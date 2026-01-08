# Train / Validation / Test Split (My Practice)

At first, I treated train/validation/test split as a fixed rule.
But I later realized that how you split data depends heavily on the task.

This note records how I usually think about it in practice.

## The basic idea

- **Training set**: used to fit the model
- **Validation set**: used to tune hyperparameters
- **Test set**: used only for final evaluation

The key rule I follow:
> The test set should not influence any modeling decisions.

## A common split ratio

In many assignments, I use something like:

- 70% training
- 15% validation
- 15% test

But this is not a rule — just a starting point.

## When things get tricky

Some cases require special care:

- **Small datasets**:  
  Cross-validation may be more reliable than a fixed split.

- **Time-series data**:  
  Random splitting can cause data leakage.  
  Temporal order must be preserved.

## A mistake I made before

I once tuned hyperparameters while repeatedly checking test performance.
That gave me an overly optimistic result.

Now I treat the test set as:
> Something I look at only once.

## When I prefer cross-validation

For small datasets, I often prefer cross-validation
because a single split can be too sensitive to randomness.
