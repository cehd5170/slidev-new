---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: true
# some information about the slides, markdown enabled
info: |
  ## Deep Learning Overview
  A comprehensive introduction to deep learning concepts and applications.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

# Deep Learning Overview

Understanding Neural Networks and AI

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
Deep learning is a subset of machine learning that uses artificial neural networks with multiple layers to model and understand complex patterns in data.
-->

---

# What is Deep Learning?

Deep learning is a powerful subset of machine learning that mimics the human brain's neural networks

<div class="grid grid-cols-2 gap-8 mt-8">

<div>

## Key Concepts

- 🧠 **Neural Networks** - Interconnected layers of artificial neurons
- 📊 **Big Data** - Requires large datasets for training
- 🔄 **Backpropagation** - Learning algorithm that adjusts weights
- 🎯 **Feature Learning** - Automatically discovers patterns in data
- ⚡ **GPU Computing** - Parallel processing for faster training

</div>

<div>

## Common Applications

- 🖼️ **Computer Vision** - Image recognition, object detection
- 🗣️ **Natural Language Processing** - Text analysis, translation
- 🎵 **Speech Recognition** - Voice assistants, transcription
- 🎮 **Game AI** - Strategic decision making
- 🚗 **Autonomous Systems** - Self-driving cars, robotics

</div>

</div>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-text-fill-color: transparent;
}
</style>

---

# Neural Network Architecture

Understanding the building blocks of deep learning models

<div class="grid grid-cols-2 gap-6 mt-6">

<div>

## Basic Structure

```python
import tensorflow as tf

# Simple neural network
model = tf.keras.Sequential([
    tf.keras.layers.Dense(128, activation='relu'),
    tf.keras.layers.Dropout(0.2),
    tf.keras.layers.Dense(64, activation='relu'),
    tf.keras.layers.Dense(10, activation='softmax')
])

# Compile the model
model.compile(
    optimizer='adam',
    loss='categorical_crossentropy',
    metrics=['accuracy']
)
```

</div>

<div>

## Layer Types

- **Dense/Fully Connected** - Every neuron connects to all neurons in next layer
- **Convolutional** - Specialized for image processing with filters
- **Recurrent (RNN/LSTM)** - Handles sequential data with memory
- **Dropout** - Prevents overfitting by randomly disabling neurons
- **Batch Normalization** - Stabilizes and speeds up training

## Training Process

1. **Forward Pass** - Data flows through network
2. **Loss Calculation** - Compare output to expected result
3. **Backward Pass** - Calculate gradients using backpropagation
4. **Weight Update** - Adjust parameters to minimize loss

</div>

</div>

---
layout: center
class: text-center
---

# The Future of Deep Learning

<div class="grid grid-cols-3 gap-8 mt-12">

<div class="text-center">

## 🚀 **Emerging Trends**

- Transformer architectures
- Self-supervised learning
- Few-shot learning
- Neural architecture search

</div>

<div class="text-center">

## 🔬 **Research Areas**

- Explainable AI
- Federated learning
- Quantum machine learning
- Neuromorphic computing

</div>

<div class="text-center">

## 🌍 **Real-world Impact**

- Healthcare diagnostics
- Climate modeling
- Drug discovery
- Scientific research

</div>

</div>

<div class="mt-16">

### Ready to dive deeper into AI and machine learning?

[TensorFlow](https://tensorflow.org) · [PyTorch](https://pytorch.org) · [Keras](https://keras.io) · [Papers With Code](https://paperswithcode.com)

</div>