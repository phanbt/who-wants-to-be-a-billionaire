# Who Wants to Be a Billionaire?

A quiz game for kids aged 8 to 12, in the style of *Who Wants to Be a Millionaire*.

## How to play

Open `index.html` in any web browser. You don't need to install anything or use the internet, except to load the fonts.

1. The game asks **10 questions**. Each question has **4 answers**, and only **1** is right.
2. The first question is worth **$10**. Each question after that is worth **double**: $10, $20, $40, $80, $160, $320, $640, $1,280, $2,560, $5,120.
3. A **right** answer adds that amount to your bank. A **wrong** answer takes the same amount away, so your bank can go below zero.
4. The best possible score is **$10,230**.

You can click the answers, or press **A–D** or **1–4** on the keyboard.

## Questions

The questions live in the `QUESTIONS` object near the top of the `<script>` in `index.html`. They are split into `easy`, `medium` and `hard`. Each game picks 4 easy, 3 medium and 3 hard questions at random, so the questions get harder as the prize goes up. The answers are shuffled every time.

To add a question, put the **correct answer first** in its list:

```js
["What is the capital of Japan?", ["Tokyo", "Kyoto", "Osaka", "Seoul"]],
```

## Play online

This repo is ready for GitHub Pages: in **Settings → Pages**, set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`. The game will then be at https://phanbt.github.io/who-wants-to-be-a-billionaire/.
