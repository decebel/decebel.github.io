---
layout: post
title: "Neural Network Gradient Descent"
comments: true
category: "Howdy+NeuralNet"
description: "Flocking behavior demo ..."
keywords: "flocking behavior, simulation, javascript, creative coding"
---

> This is a placeholder for flocking behavior simulation for **Art+Code**, inspired by many sources and implemented in javascript.

Learning NN the easy way.
In Keras, why do we need to provide an output when the input_dim is provided. And when can this be different from the provided input.

For example:
model = Sequential()
model.add(Dense(12, input_dim=8, init='uniform', activation='relu'))

Here the input is 8 features, so the output should be 8 too. But the output is 12 instead. 
Seems what is happening is:
[input: 8 features -> InputLayer -> output: 8 features ] -> [input: 8 -> Dense -> output: 12]








<paragraph>
How do we visualize the model:

To any model you build, do the following:
<pre><code>
from keras.utils.visualize_util import plot
plot(model, show_shapes=True, to_file='model.png')
</code>
</pre>
If you are on mac, you need to install pydot and graphviz.

for graphviz, 
<pre><code>
brew install graphviz
</code>
</pre>

for pydot
<pre><code>
conda install pydot
</code>
</pre>


</paragraph>
