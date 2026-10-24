# ML Foundations demos

Browser demos for 기계학습기초 — ML Foundations (Hongik University, 2026-2).
Each demo is one self-contained HTML file: no server, no libraries, no network.

Published with GitHub Pages at <https://hongik-aicourses.github.io/ml-demos/>.

| Week | Demo | Page |
|---|---|---|
| 4, Hour 1 | Linear regression with gradient descent, line by line | [week04-gradient-descent/](https://hongik-aicourses.github.io/ml-demos/week04-gradient-descent/) |
| 4, Hour 2 | Logistic regression with gradient descent, line by line | [week04-logistic-regression/](https://hongik-aicourses.github.io/ml-demos/week04-logistic-regression/) |
| 4, Hour 3 | Evaluating a classifier: the threshold, the confusion matrix, precision, recall and the ROC curve | [week04-evaluation/](https://hongik-aicourses.github.io/ml-demos/week04-evaluation/) |
| 5, Hour 1 | Softmax regression | [week05-softmax/](https://hongik-aicourses.github.io/ml-demos/week05-softmax/) |
| 5, Hour 2 | Entropy, cross-entropy and KL | [week05-losses/](https://hongik-aicourses.github.io/ml-demos/week05-losses/) |
| 5, Hour 3 | The multilayer perceptron | [week05-mlp/](https://hongik-aicourses.github.io/ml-demos/week05-mlp/) |
| 5, make-up hour | Backpropagation | [week05-backprop/](https://hongik-aicourses.github.io/ml-demos/week05-backprop/) |
| 6, Hour 3 | Training a deep network: the starting weights, the activation and the scale of the inputs | [week06-training/](https://hongik-aicourses.github.io/ml-demos/week06-training/) |
| 7, Hour 1 | A bigram language model, line by line: counting letter pairs in 240 names, add-one smoothing, sampling and perplexity | [week07-bigram/](https://hongik-aicourses.github.io/ml-demos/week07-bigram/) |
| 7, Hour 1 | Word vectors: nearest words, analogies and a two-dimensional map (GloVe 6B, 50 dimensions) | [week07-word-vectors/](https://hongik-aicourses.github.io/ml-demos/week07-word-vectors/) |
| 7, Hour 2 | Training a character MLP language model: three letters of context, a two-number embedding per character, minibatch SGD line by line, a weight decay setting; the loss curves and sampled names | [week07-mlp-lm/](https://hongik-aicourses.github.io/ml-demos/week07-mlp-lm/) |
| 8, Hour 1 | Byte pair encoding, merge by merge: d2l's four words or The Time Machine, the most frequent pair merged, the segmentation of a new word | [week08-bpe/](https://hongik-aicourses.github.io/ml-demos/week08-bpe/) |
| 8, Hour 3 | A recurrent language model, step by step: the hidden state after each character, backpropagation through time, gradient clipping, sampled names | [week08-rnn/](https://hongik-aicourses.github.io/ml-demos/week08-rnn/) |
| 8, make-up | How much to trust a test loss: test sets drawn from per-token losses, the standard error, the normal curve, how often 95% intervals contain the mean | [error-bars/](https://hongik-aicourses.github.io/ml-demos/error-bars/) |
| 9, Hour 1 | Attention pooling, line by line: Nadaraya-Watson regression and scaled dot-product attention; scores, softmax weights, the weighted average | [week09-attention/](https://hongik-aicourses.github.io/ml-demos/week09-attention/) |
| 9, Hour 2 | Self-attention on a sentence: queries, keys and values, the causal mask, the softmax row by row, RoPE and its invariance to shifting positions | [week09-self-attention/](https://hongik-aicourses.github.io/ml-demos/week09-self-attention/) |
| 9, Hour 3 | Why the block has a residual stream: activations and gradients through a deep stack, plain or residual, with or without RMSNorm | [week09-block/](https://hongik-aicourses.github.io/ml-demos/week09-block/) |
| 9, make-up | Fine-tuning a model to follow a prompt: prompt tokens as new rows, the loss masked on the prompt, sampled names before and after SFT | [instruction-tuning/](https://hongik-aicourses.github.io/ml-demos/instruction-tuning/) |
| later | Regularization: weight decay and L1 on a polynomial | [week06-regularization/](https://hongik-aicourses.github.io/ml-demos/week06-regularization/) |
| later | A convolution, line by line: a 3 &times; 3 filter over a picture, then a causal filter over a sentence | [convolution/](https://hongik-aicourses.github.io/ml-demos/convolution/) |
| later | A small CNN learns its own filters: 8 filters on handwritten digits, next to softmax regression, with moved digits | [cnn-digits/](https://hongik-aicourses.github.io/ml-demos/cnn-digits/) |
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

- **Bigram model:** the stepper follows the Week 4 demos (from *Machine Learning From Scratch, Part 1* by
  [@machinelearningtogo](https://www.tiktok.com/@machinelearningtogo)); the model and Laplace smoothing follow d2l.ai 9.3.
- **Word vectors:** GloVe 6B, 50 dimensions (Pennington, Socher and Manning, 2014), released under the Open
  Data Commons Public Domain Dedication and License; the 10,000 most frequent words, alphabetic ones only,
  stored to 8 bits. Similarity and analogies follow d2l.ai 15.7.
- **Convolutional networks (both pages):** these follow the short videos *Machine Learning
  From Scratch, Part 32: CNN* and *Part 10: How AI Sees* by
  [@machinelearningtogo](https://www.tiktok.com/@machinelearningtogo) and *Convolutional Neural
  Network: how the kernel really works* by
  [@DataScienceFoundry](https://www.tiktok.com/@datasciencefoundry) on TikTok: the 8 &times; 8
  digit, the 3 &times; 3 filter that multiplies and adds, the feature map, 2 &times; 2 max pooling,
  8 learned filters (72 numbers), the comparison of 72 shared weights with 4,608, and each
  digit's weights drawn as a stencil. The pages add the sentence (a causal filter over
  character vectors) and the test with moved digits. Digits: UCI Optical Recognition of
  Handwritten Digits (Alpaydin and Kaynak), CC BY 4.0, as shipped with scikit-learn.

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
