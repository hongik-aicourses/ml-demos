# ML Foundations demos

Browser demos for 기계학습기초 — ML Foundations (Hongik University, 2026-2).
Each demo is one self-contained HTML file: no server, no libraries, no network.

Published with GitHub Pages at <https://hongik-aicourses.github.io/ml-demos/>.

| Week | Demo | Page |
|---|---|---|
| 4, Hour 1 | Linear regression with gradient descent, line by line | [week04-gradient-descent/](https://hongik-aicourses.github.io/ml-demos/week04-gradient-descent/) |
| 4, Hour 2 | Logistic regression with gradient descent, line by line | [week04-logistic-regression/](https://hongik-aicourses.github.io/ml-demos/week04-logistic-regression/) |
| 4, Hour 3 | Evaluating a classifier: the threshold, the confusion matrix, precision, recall and the ROC curve | [week04-evaluation/](https://hongik-aicourses.github.io/ml-demos/week04-evaluation/) |
| later | Naive Bayes spam filter, clue by clue | [naive-bayes/](https://hongik-aicourses.github.io/ml-demos/naive-bayes/) |

## Where the files come from

This repository is a published copy. The source of each demo is kept in the course's
instructor repository (`examples/current/weekNN_*.html`); edit it there and copy it here,
rather than editing this repository directly.

## Credit

- **Gradient descent (Week 4, Hour 1) and logistic regression (Hour 2):** these follow
  the short video *Machine Learning From Scratch, Part 1* by
  [@machinelearningtogo](https://www.tiktok.com/@machinelearningtogo) on TikTok: the
  thirteen-line loop, the order in which its steps are shown, and its eight data points
  (x = 1, …, 8; y = 2.9, 3.4, 4.9, 4.7, 6.2, 6.9, 7.3, 8.6). The logistic-regression page
  reuses that stepper with its own labels.
- **Naive Bayes:** this follows the short video *Naive Bayes* by
  [@DataScienceFoundry](https://www.tiktok.com/@datasciencefoundry) on TikTok: its word
  table, the prior of 25%, the example email and the order of the explanation. The page adds
  the two words of the email the video leaves uncounted ("claim", "prize") and the log-odds
  view.

## License

© 2026 Kuk Jin Jang, Hongik University.

Everything in this repository — the code and the text alike — is licensed under
[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) (full text in
`LICENSE`):

- **you may** share and adapt it for non-commercial purposes, such as teaching and
  study, provided you give credit and release any adaptation you share under the same
  license;
- **commercial use** and **closed-source use** are not granted by the license. For
  either, or for any other licensing, ask: jangkj@hongik.ac.kr.

The credited videos and their authors are not covered by this license.
