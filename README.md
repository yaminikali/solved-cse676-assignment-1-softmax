Download Link: https://assignmentchef.com/product/solved-cse676-assignment-1-softmax
<br>
<h1>Softmax</h1>

<ul>

 <li> Prove that softmax is invariant to constant sifts in the input, <em>e.</em>, for any input vector <strong>x </strong>and a constant scalar <em>c</em>, the following holds:</li>

</ul>

softmax(<strong>x</strong>) = softmax(<strong>x</strong>+<em>c</em>) <em>,</em>

where softmax(<strong>x</strong>), and <strong>x</strong>+<em>c </em>means adding <em>c </em>to every dimension of <strong>x</strong>.

<ul>

 <li> Let <strong>z </strong>= <strong>Wx</strong>+<strong>c</strong>, where <strong>W </strong>and <strong>c </strong>are some matrix and vector, respectively. Let</li>

</ul>

<em>J </em>= <sup>X</sup>logsoftmax(<strong>z</strong>)<em><sub>i </sub>.</em>

<em>i</em>

Calculate the derivatives of <em>J </em>w.r.t. <strong>W </strong>and <strong>c</strong>, respectively, <em>i.e.</em>, calculate <em><sub>∂</sub><u><sup>∂J</sup></u></em><strong><sub>W </sub></strong>and .

<h1>0.2        Logistic Regression with Regularization</h1>

<ul>

 <li>[10 point] Let the data be (, where <strong>x</strong><em><sub>i </sub></em>∈ R<em><sup>d </sup></em>and <em>y<sub>i </sub></em>∈ {0<em>,</em>1}. Logistic regression is a binary classification model, with the probability of <em>y<sub>i </sub></em>being 1 as:</li>

</ul>

where <em>θ </em>is the model parameter. Assume we impose an <em>L</em><sub>2 </sub>regularization term on the parameter, defined as:

with a positive constant <em>λ</em>. Write out the final objective function for this logistic regression with regularization model.

<ul>

 <li>[10 point] If we use gradient descent to solve the model parameter. Derive the updating rule for <em>θ</em>. Your answer should contain the derivation, not just the final answer.</li>

</ul>

<h1>0.3        Derivative of the Softmax Function</h1>

1) [10 point] Define the loss function as

<em>K</em>

<em>J</em>(<strong>z</strong>) = −<sup>X</sup><em>y<sub>k </sub></em>log ˜<em>y<sub>k </sub>,</em>

<em>k</em>=1

where ˜          , and (<em>y</em><sub>1</sub><em>,</em>··· <em>,y<sub>K</sub></em>) is a known probability vector. Derive the .

Note <strong>z </strong>= (<em>z</em><sub>1</sub><em>,</em>··· <em>,z<sub>K</sub></em>) is a vector so <em><sup>∂J</sup></em><em><sub>∂</sub></em><sup>(</sup><strong><sub>z</sub><sup>z</sup></strong><sup>) </sup>is in the form of a vector. Your answer should contain the derivation, not just the final answer.

1

CSE 676                                                      <strong>Changyou Chen                                   </strong>Spring 2021

2 [10 point] Assume the above softmax is the output layer of an FNN. Briefly explain how the derivative is used in the backpropagation algorithm.

3) [10 points] Let <strong>z </strong>= <strong>W</strong><em><sup>T </sup></em><strong>h</strong>+<strong>b</strong>, where <strong>W </strong>is a matrix, <strong>b </strong>and <strong>h </strong>are vectors. Use the chain rule to calculate the gradient of <strong>W </strong>and <strong>b</strong>, <em>i.e.</em>, <em><sub>∂</sub><u><sup>∂J</sup></u></em><strong><sub>W </sub></strong>and, respectively.

<h1>0.4         MNIST with FNN</h1>

1) [30 points] Design an FNN for MNIST classification. Implement the model and plot two curves in one figure: <em>i</em>) training loss vs. training iterations; <em>ii</em>) test loss vs. training iterations.

<ul>

 <li>You can use online code. However, you must reference (cite) the code in your answer.</li>

 <li>Submission includes the plot of the two curves and the runnable code (with a ReadMe file containing instructions on how to run the code).</li>

</ul>