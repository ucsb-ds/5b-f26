---
parent: PrairieLearn
layout: default
title: "practice-quiz-04"
description:  "Study Guide"
---

## 5b-f26 practice-quiz-05 student guide

This guide is for students taking **Practice Quiz 5** in CMPSC 5B (Fall 2026),
the second practice quiz for the midterm. For each question on the quiz it
tells you which part of the labs, and which sections of the textbook, teach
the material you need. If a question gives you trouble, go back to that lab
section and reread the textbook section, then try the question again (you get
a fresh random version each time).

The textbook is *Computational and Inferential Thinking: The Foundations of
Data Science*, 2nd edition, free online at <https://inferentialthinking.com/>.
Lab sections refer to the numbered headings inside each lab notebook
(`lab02.ipynb`, `lab03.ipynb`, `lab04.ipynb`).

The quiz has ten questions worth 10 points each, grouped by lab. Three of the
slots (2, 3 and 5) hold a small set of closely related questions; the quiz
gives you **one** question from the set, and a classmate may get a different
one. The table lists every question that can appear in a slot, so practice
all of them.

| # | Question (as titled on the quiz) | Lab and section | Textbook sections |
|---|---|---|---|
| 1 | lab02c: table operations | **Lab 2**, Section 3 *Table Operations* (Questions 3.2 `num_rows`, 3.3 `select`, 3.5 `sort`) and Section 4 (Questions 4.1 and 4.2: chained `where` and a proportion). The `where` conditions on the quiz are deliberately different from the lab's, so read each condition carefully and pick the matching `are.` predicate from the reminder table in the notebook | [3.4 Introduction to Tables](https://inferentialthinking.com/chapters/03/4/introduction-to-tables), [6 Tables](https://inferentialthinking.com/chapters/06/tables), [6.1 Sorting Rows](https://inferentialthinking.com/chapters/06/1/sorting-rows), [6.2 Selecting Rows](https://inferentialthinking.com/chapters/06/2/selecting-rows) |
| 2 | one of: lab03a: strings containing quotation marks | **Lab 3**, Section 1 *Text* (Question 1.1, the Gagarin conversation) | [4.2 Strings](https://inferentialthinking.com/chapters/04/2/strings), [3.2 Names](https://inferentialthinking.com/chapters/03/2/names) |
|   | lab03b: the replace string method | **Lab 3**, Section 1.1 *String Methods* (Question 1.1.1, `hitchhiker` to `matchmaker`) | [4.2.1 String Methods](https://inferentialthinking.com/chapters/04/2/1/string-methods), [3.3 Call Expressions](https://inferentialthinking.com/chapters/03/3/calls) |
|   | lab03d: len of a string | **Lab 3**, Section 1.3 *Passing strings to functions* (Question 1.3.1) | [4.2 Strings](https://inferentialthinking.com/chapters/04/2/strings), [3.3 Call Expressions](https://inferentialthinking.com/chapters/03/3/calls) |
| 3 | one of: lab03e: make_array with numbers and math constants | **Lab 3**, Section 2.1 *Making arrays* (Question 2.1.1); **Lab 2**, Section 2 for `math.pi` and `math.e` | [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays), [5 Sequences](https://inferentialthinking.com/chapters/05/sequences), [4.1 Numbers](https://inferentialthinking.com/chapters/04/1/numbers) |
|   | lab03f: make_array with strings | **Lab 3**, Section 2.1 *Making arrays* (Question 2.1.2, the `"Hello"`, `","`, `" "`, `"world"`, `"!"` array) | [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays), [5 Sequences](https://inferentialthinking.com/chapters/05/sequences), [4.2 Strings](https://inferentialthinking.com/chapters/04/2/strings) |
| 4 | lab03h: item, indexing an array | **Lab 3**, Section 2.2 *Working with single elements of arrays (indexing)* (Question 2.2.1, `population_1973`) | [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays), [5 Sequences](https://inferentialthinking.com/chapters/05/sequences) |
| 5 | one of: lab03i: np.round on an array | **Lab 3**, Section 2.3 *Doing something to every element of an array* (Question 2.3.1, `population_rounded`) | [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays), [5 Sequences](https://inferentialthinking.com/chapters/05/sequences) |
|   | lab03n: elementwise arithmetic on a small array | **Lab 3**, Section 5.2 *Doing something to every element of an array (cont.)* (Question 5.2.1, `total_charges` with a tip) | [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays), [5 Sequences](https://inferentialthinking.com/chapters/05/sequences) |
| 6 | lab03j: Table().with_columns | **Lab 3**, Section 3 *Creating Tables* (Question 3.1, `top_10_movies` from two arrays) | [6 Tables](https://inferentialthinking.com/chapters/06/tables), [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays) |
| 7 | lab03k: load imdb, averages by period, remainder count | **Lab 3**, Section 3 *Creating Tables*, the part on loading a table from a file (Question 3.2) and Section 4 *More Table Operations!* (Question 4.2, average rating before and after a year; Question 4.3, counting years with `%`) | [6 Tables](https://inferentialthinking.com/chapters/06/tables), [6.2 Selecting Rows](https://inferentialthinking.com/chapters/06/2/selecting-rows), [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays), [3.3 Call Expressions](https://inferentialthinking.com/chapters/03/3/calls) |
| 8 | lab04c: a function that prints, print_kth_top_movie_year | **Lab 4**, Section 1 *Defining functions*, the `movies_by_year` worked example, Question 1.4, and the text after it on `print` versus `return` | [8 Functions and Tables](https://inferentialthinking.com/chapters/08/functions-and-tables), [6.1 Sorting Rows](https://inferentialthinking.com/chapters/06/1/sorting-rows), [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays), [3.3 Call Expressions](https://inferentialthinking.com/chapters/03/3/calls) |
| 9 | lab04d: from a pay string to a conversion function | **Lab 4**, Section 2 *Functions and CEO Incomes* (Questions 2.1 to 2.4: `type`, extracting a pay string, `strip` and `float`, then `convert_pay_string_to_number`) | [4 Data Types](https://inferentialthinking.com/chapters/04/data-types), [4.2 Strings](https://inferentialthinking.com/chapters/04/2/strings), [4.2.1 String Methods](https://inferentialthinking.com/chapters/04/2/1/string-methods), [8 Functions and Tables](https://inferentialthinking.com/chapters/08/functions-and-tables), [6 Tables](https://inferentialthinking.com/chapters/06/tables) |
| 10 | lab04f: applying functions to the CEO pay table | **Lab 4**, Section 3 *`apply`ing functions* (Questions 3.2 to 3.6: `apply`, `with_column`, an average, a proportion, `where` with `are.not_equal_to`) | [8.1 Applying a Function to a Column](https://inferentialthinking.com/chapters/08/1/applying-a-function-to-a-column), [8 Functions and Tables](https://inferentialthinking.com/chapters/08/functions-and-tables), [6 Tables](https://inferentialthinking.com/chapters/06/tables), [6.2 Selecting Rows](https://inferentialthinking.com/chapters/06/2/selecting-rows), [5.1 Arrays](https://inferentialthinking.com/chapters/05/1/arrays) |

### Tips

* Every question on this quiz opens a Jupyter notebook in a separate tab.
  Put your answers in the code cells that start with `#grade`, save the
  notebook, then come back to PrairieLearn and click **Save and Grade**.
  Several questions have more than one `#grade` cell; each is graded
  separately, so partial credit is possible.
* When a question uses a data file (`imdb.csv`, `world_population.csv`,
  `movies_by_year.csv`, `raw_compensation.csv`), the file is already in the
  notebook's folder and a provided cell loads it. The data is a random
  sample, so your numbers will not match the lab's; the method is what
  matters.
* Arrays: `np.arange` and `make_array` build them, `item(i)` reads one
  element (counting from 0), and arithmetic or `np.round` applied to an
  array works on every element at once.
* Tables: `where` keeps rows, `column` turns one column into an array, and
  `item(0)` or `np.average` turns that array into a single number. Watch
  the boundary words ("before 2000" versus "2000 or after").
* Functions: a function that **prints** returns `None`; a function that
  **returns** gives a value you can store. Inside the body, use the
  parameter, not a variable from outside the function. Passing a function
  to `apply` means writing its name without parentheses.