# Confusion Matrix (My Understanding)

I used to mix up TP, FP, TN, and FN during exams, especially under time pressure.
This note is written to fix that problem permanently.

## Basic layout

|              | Predicted Positive | Predicted Negative |
|--------------|--------------------|--------------------|
| Actual Positive | TP | FN |
| Actual Negative | FP | TN |

## The way I remember it

- **TP**: model says positive, and it really is
- **FP**: model says positive, but it is not (false alarm)
- **FN**: model misses a positive case

The key idea is simple:
> FP and FN are both mistakes, but in opposite directions.

## A mistake I made before

I used to confuse FP and FN when reading word problems.
Now I always ask myself:
1. Did the model say positive?
2. Was it actually positive?
