## 1. Introduction

#### What is your MSE/MAE with linreg vs tuned network?

---

Linreg: 26.61 (MSE), 3.6467 (MAE)

Tuned: 

![img.png](img/1a.png)

#### What happens to your train and test results if you add 5 hidden layers with 128 neurons each?

---

![img.png](img/1b.png)

NOTE: Though in most cases adding the layers slightly improved the results, the variance of outcomes may be drastic. 
If the initial guess is off, the weights will converge to the incorrect local minima, leaving our prediction poor. 
This being said, the more layers, the more complexity, and the solution in part A was often near or better than that of 
part B, with _less_ variance, therefore I would leave out these extra hidden layers.

![img.png](img/1b_bad.png)

## 2. Intro to convolution operations: padding

#### What is a response layer? (Give a brief, 1-sentence description)

---

- After a conv2D map is applied to a network, the 2D "filters" which are stacked are known as response layers.

#### Given the filter shape of (26, 26, 32), what does each number represent?

---

- (modified width, modified height, number of responses)

#### Given 6x6 input and filter of (3,3): what is the response shape that we get? 

---

(4,4,25)

#### Given (33, 33, 1) input and filter of (2,2): what is the response shape that we get?

---

- (32, 32, 1024)

#### What is the difference between ‘valid’ and ‘same’ padding? 

---

- valid: No padding on original input layer
- same: pad original network so that output (w,h) is the same as the input layer.

## 3. Convolution parameters: stride and pooling

#### What is max pooling? (Give a brief, 1-sentence description)

---

- When applying convolution to a network, each response takes the maximum value found within the filter.

#### If I apply pooling of 2 ((2,2) window with a stride of 2) to a (6,6) array, what is the resulting size?

---

- (3, 3, 9)


## 4. ConvNet Architectures, layers


## 5. Practical patterns
