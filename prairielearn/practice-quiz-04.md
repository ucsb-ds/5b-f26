---
parent: PrairieLearn
layout: default
title: "practice-quiz-04"
description:  "Study Guide"
---


## 5b-f26 practice-quiz-04 student guide

This guide is for students taking **Practice Quiz 4** in CMPSC 5B (Fall 2026).
For each question on the quiz it tells you which part of the labs, and
which sections of the textbook, teach the material you need. If a question
gives you trouble, go back to that lab section and reread the textbook
section, then try the question again (you get a fresh random version each
time).

The textbook is *Computational and Inferential Thinking: The Foundations of
Data Science*, 2nd edition, free online at <https://inferentialthinking.com/>.
Lab sections refer to the numbered headings inside each lab notebook
(`lab01.ipynb`, `lab02.ipynb`, and so on).

The questions appear on the quiz in roughly the order the material comes up
in the labs.

| # | Question (as titled on the quiz) | Lab and section | Textbook sections |
|---|---|---|---|
| 1 | lab01a: Arithmetic expression | **Lab 1**, Section 2.1 *Arithmetic* and Section 3 *Names* (Question 2.1.1) | [3.1 Expressions](https://inferentialthinking.com/chapters/03/1/expressions), [3.2 Names](https://inferentialthinking.com/chapters/03/2/names) |
| 2 | lab01b: Seconds in a span of years | **Lab 1**, Section 3.1 *Checking Your Code* (Question 3.1.2, `seconds_in_a_decade`) | [3.1 Expressions](https://inferentialthinking.com/chapters/03/1/expressions), [3.2 Names](https://inferentialthinking.com/chapters/03/2/names) |
| 3 | lab01c: Apollo 15 hammer drop | **Lab 1**, Section 3.3 *Application: A Physics Experiment* (Questions 3.3.1 and 3.3.2) | [3.1 Expressions](https://inferentialthinking.com/chapters/03/1/expressions), [3.2 Names](https://inferentialthinking.com/chapters/03/2/names), [4.1 Numbers](https://inferentialthinking.com/chapters/04/1/numbers) |
| 4 | lab01d: Manhattan walking distance with abs | **Lab 1**, Section 4 *Calling Functions* and 4.1 *Application: Computing Walking Distances* (Question 4.1.1) | [3.3 Call Expressions](https://inferentialthinking.com/chapters/03/3/calls) |
| 5 | lab01e: Nested expressions, smallest difference of cat lengths | **Lab 1**, Section 5 *Understanding Nested Expressions* and 5.1 *More Nesting* (Question 5.1.1) | [3.3 Call Expressions](https://inferentialthinking.com/chapters/03/3/calls) |
| 6 | Show results of sort by dragging blocks (Cars or Skyscrapers) | **Lab 2**, Section 3 *Table Operations*, the part on `sort` and `descending=True` | [6.1 Sorting Rows](https://inferentialthinking.com/chapters/06/1/sorting-rows); background in [3.4 Introduction to Tables](https://inferentialthinking.com/chapters/03/4/introduction-to-tables) and [6 Tables](https://inferentialthinking.com/chapters/06/tables) |
| 7 | Python Expressions: strings, ints and the + operator | **Lab 3**, Section 1 *Text* and Section 1.2 *Converting to and from Strings* (the `8 + "8"` example and the `int` / `float` / `str` table); **Lab 1**, Section 2.1 for adding two numbers | [4.2 Strings](https://inferentialthinking.com/chapters/04/2/strings), [4.1 Numbers](https://inferentialthinking.com/chapters/04/1/numbers), [3.1 Expressions](https://inferentialthinking.com/chapters/03/1/expressions) |
| 8 | Numpy Expressions: arange | **Lab 3**, Section 2.1 *Making arrays*, the `np.arange` part (Question 2.1.3), and Section 5.1 *`np.arange` (cont.)*; the one-argument form `np.arange(5)` shows up in **Lab 5** | [5.2 Ranges](https://inferentialthinking.com/chapters/05/2/ranges), [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays) |
| 9 | Type Evaluation | **Lab 4**, Section 2 *Functions and CEO Incomes* (the `type` function, Question 2.1); **Lab 3**, Section 1.2 for `int`, `float` and `str`; **Lab 5**, Section 1 for `bool` values from comparisons | [4 Data Types](https://inferentialthinking.com/chapters/04/data-types), [4.1 Numbers](https://inferentialthinking.com/chapters/04/1/numbers), [4.2 Strings](https://inferentialthinking.com/chapters/04/2/strings), [4.3 Comparisons](https://inferentialthinking.com/chapters/04/3/comparison) |
| 10 | Define function abs_value_diff | **Lab 4**, Section 1 *Defining functions* (`def`, the signature, the body, `return`); **Lab 6**, Question 1.5 (the `statistic` function); **Lab 1**, Section 4 for `abs` | [8 Functions and Tables](https://inferentialthinking.com/chapters/08/functions-and-tables), [8.1 Applying a Function to a Column](https://inferentialthinking.com/chapters/08/1/applying-a-function-to-a-column), [3.3 Call Expressions](https://inferentialthinking.com/chapters/03/3/calls) |

### Tips

* Questions 1 to 5 and 10 open a Jupyter notebook in a separate tab. Put
  your answer in the code cell that starts with `#grade`, save the notebook,
  then come back to PrairieLearn and click **Save and Grade**.
* Questions 7 and 8 ask you to work out values by hand. The key facts are
  that `+` adds two numbers but joins two strings and is an error for one
  of each, and that `np.arange` never includes its stop value.
* For question 6, remember that text sorts alphabetically and numbers sort
  numerically, and that `sort` goes from smallest to largest unless you
  pass `descending=True`.

