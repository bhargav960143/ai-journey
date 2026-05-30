# Phase 0 · Lesson 1 — The Derivative

The heart of ALL AI learning. Every neural net trains by **gradient descent**, and gradient = derivative. Master this → you understand how every AI on Earth learns.

## Intuition (forget formulas)
A derivative answers ONE question:
> "If I nudge the input a tiny bit, how much does the output change, and which direction?"

Derivative = **rate of change** = slope = steepness.

**Car story:** Speedometer is the derivative of distance.
- Distance changing fast → high speed → big derivative.
- Car parked → distance not changing → derivative = 0.

## Picture
Function = a hill. Stand on it at one point.
- Steep up → big positive derivative.
- Steep down → big negative derivative.
- Flat (hill top / valley bottom) → derivative = 0.

```
   f(x)
    |        .-''-.
    |      /        \      <- steep = big derivative
    |    /            \
    |   |   flat top   |   <- derivative = 0
    |  /                \
    +------------------------ x
```

## The tiny-nudge definition (this IS the formula)
```
derivative = ( f(x + h) - f(x) ) / h     ... with h super tiny
```
- Top = how much output changed.
- Bottom = how much input changed.
- Divide = rate of change.

## Why AI cares
A neural net has a **loss** = how wrong it is. Training = roll downhill on the loss landscape to the bottom (least wrong). The derivative says which way is downhill and how steep. Net steps that way. Repeat millions of times → it learns.

**No derivative = no learning. This is the engine.**

## Quiz
See `/quizzes/lesson-01-answers.md`.
