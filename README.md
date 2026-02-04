
---
Did you know that calc was short for calculator?
---

## Why This Project Exists

The goal is to:
- understand neural network limitations
- observe extrapolation failure
- explore confidence estimation
- contrast machine learning with symbolic reasoning

---

## How to Run

1. Open `RNGCalc.ipynb`
2. Run all cells top to bottom
3. Use the interactive prompt at the end to test inputs

Works best in **Google Colab** or a local Python environment with PyTorch.

---

## The Architecture of Anxiety

Most calculators use logic. RNGCalc just gambles technically.

I trained a simple Feed-Forward Network on 8,000 arithmetic pairs.
- **The Catch:** I trained it on numbers between `-10` and `10`.
- **The Result:** When you ask it to solve `100 * 100`, it tries to extrapolate, fails miserably, and has an existential crisis.

### The "Confidence" Algorithm
Instead of an LLM, I used a deterministic ratio-based confidence system because I couldn't bother with api calls:
`Confidence = min(|Actual|, |Pred|) / max(|Actual|, |Pred|) * 100`

If the model is wrong, it knows it's wrong, and the hardcoded commentary reflects that terror.

## Disclaimer

This calculator should not be used for:
- anything important

This calculator can be used for:
- taxes (in the same way a coin flip can be used for taxes)

Math was harmed in the making of this project.



<img width="420" height="71" alt="image" src="https://github.com/user-attachments/assets/1352f53a-b0d2-4cd5-81dc-8c7178c13244" />
<img width="1589" height="1229" alt="image" src="https://github.com/user-attachments/assets/0721620a-50a4-48b8-b06f-a469bec01cfb" />


