# ReLU_Plus_Plus

ReLU++: A modified ReLU activation function with enhanced performance for deep learning models.

An improved implementation of the ReLU activation function, with an adjustable slope for positive and negative values.

_Description_

The ReLU (Rectified Linear Unit) activation function is one of the most popular in deep neural networks. However, it has some limitations, such as the loss of information in negative values.

ReLU_Plus_Plus is a variant of the ReLU function that attempts to mitigate these limitations. It allows adjusting the slope for positive and negative values, which can improve the performance of neural networks in certain tasks.

_Formula_

The ReLU_Plus_Plus function is defined as:

If x < 0, then f(x) = ax

If x ≥ 0, then f(x) = bx

Where a and b are parameters that control the slope for negative and positive values, respectively.

It is important to note that ReLU (a=0, b=1), Leaky ReLU (a=0.01, b=1), and Parametric ReLU (a=0.05, b=1) are special cases of ReLU++, making ReLU++ a more flexible and efficient generalization of these activation functions. Additionally, when in ReLU++ a=1 and b=1, the activation function behaves like an identity function, meaning that the output is equal to the input, effectively "disabling" the activation function.

_Features_

- Adjustable slope for positive and negative values
- Compatible with major machine learning libraries (TensorFlow, PyTorch, etc.)
- Easy to implement and use

_Installation_

To install ReLU_Plus_Plus, you can use the following command:

```
git clone https://github.com/aluminarius/ReLU_Plus_Plus.git
```

_Usage_

To use ReLU_Plus_Plus in your machine learning models, simply import the function and use it like any other activation function:

```
from relu_plus_plus import ReLU_Plus_Plus

Create a machine learning model
model = tf.keras.models.Sequential([
    tf.keras.layers.Dense(64, activation=ReLU_Plus_Plus(a=0.1, b=0.5)),
    tf.keras.layers.Dense(10, activation='softmax')
])
```

_Contribution_

ReLU_Plus_Plus is an open-source project, and any contribution is welcome. If you want to contribute, please fork the repository and submit a pull request.

_Authors_
- Alex
- Lumin

_License_

ReLU_Plus_Plus is distributed under the MIT license.
