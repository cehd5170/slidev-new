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
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Deep Learning Overview
  A comprehensive introduction to deep learning concepts and applications.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

# Welcome to Deep Learning

Understanding Neural Networks and Modern AI

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/tensorflow/tensorflow" target="_blank" alt="TensorFlow"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
Deep learning is revolutionizing how machines understand and process information, from computer vision to natural language processing.
-->

---

# What is Deep Learning?

Deep learning is a powerful subset of machine learning inspired by the human brain, consisting of the following key aspects

- 🧠 **Neural Networks** - multi-layered artificial neurons that process information
- 📊 **Pattern Recognition** - automatically discovers complex patterns in data
- 🔄 **Backpropagation** - learning algorithm that optimizes network weights
- 🎯 **Feature Learning** - extracts meaningful representations without manual engineering
- ⚡ **Scalability** - leverages GPU computing for massive parallel processing
- 🌐 **Versatility** - applicable across vision, language, speech, and decision-making

<br>
<br>

Read more about [Why Deep Learning?](https://www.deeplearningbook.org/)

<!--
Deep learning has transformed AI by enabling machines to learn hierarchical representations of data, leading to breakthroughs in computer vision, natural language processing, and many other domains.
-->

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
layout: image-right
image: https://source.unsplash.com/1920x1080/?artificial-intelligence,neural-network
---

# Neural Architecture

Build powerful models with layered networks![^1]

```python {all|2|1-6|9|all}
import tensorflow as tf

# Define neural network layers
model = tf.keras.Sequential([
    tf.keras.layers.Dense(128, activation='relu'),
    tf.keras.layers.Dropout(0.2),
    tf.keras.layers.Dense(64, activation='relu'),
    tf.keras.layers.Dense(10, activation='softmax')
])

# Compile and train
model.compile(optimizer='adam',
              loss='categorical_crossentropy',
              metrics=['accuracy'])
```

<arrow v-click="3" x1="400" y1="420" x2="230" y2="330" color="#564" width="3" arrowSize="1" />

[^1]: [Learn More](https://www.tensorflow.org/guide/keras)

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

---
layout: center
class: text-center
---

# The Future is Here

<div class="grid grid-cols-2 gap-8 pt-4">

<div>

## Deep Learning Process

<div class="flowchart">
  <div class="flow-step start">
    <div class="box">Raw Data</div>
    <div class="arrow">↓</div>
  </div>
  
  <div class="flow-step">
    <div class="box">Data Preprocessing</div>
    <div class="arrow">↓</div>
  </div>
  
  <div class="flow-step">
    <div class="box neural">Neural Network Training</div>
    <div class="arrow">↓</div>
  </div>
  
  <div class="flow-step">
    <div class="diamond">Training Complete?</div>
    <div class="decision-arrows">
      <div class="arrow-left">← No</div>
      <div class="arrow-down">↓ Yes</div>
    </div>
  </div>
  
  <div class="flow-step">
    <div class="box success">Model Deployment</div>
  </div>
</div>

</div>

<div>

## Applications

<div class="applications-grid">
  <div class="app-category vision">
    <h4>Computer Vision</h4>
    <ul>
      <li>Image Recognition</li>
      <li>Medical Diagnosis</li>
      <li>Autonomous Vehicles</li>
    </ul>
  </div>
  
  <div class="app-category nlp">
    <h4>Natural Language</h4>
    <ul>
      <li>ChatGPT & LLMs</li>
      <li>Language Translation</li>
      <li>Text Summarization</li>
    </ul>
  </div>
  
  <div class="app-category rl">
    <h4>Reinforcement Learning</h4>
    <ul>
      <li>Game AI (AlphaGo)</li>
      <li>Robotics Control</li>
      <li>Trading Systems</li>
    </ul>
  </div>
  
  <div class="app-category gen">
    <h4>Generative AI</h4>
    <ul>
      <li>AI Art & Images</li>
      <li>Music Generation</li>
      <li>Code Generation</li>
    </ul>
  </div>
</div>

</div>

</div>

<div class="mt-6 text-center">

**Ready to build the future with AI?**

[TensorFlow](https://tensorflow.org) · [PyTorch](https://pytorch.org) · [Hugging Face](https://huggingface.co) · [Papers With Code](https://paperswithcode.com)

</div>

<style>
.flowchart {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
  margin: 20px 0;
}

.flow-step {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.box {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 12px 20px;
  border-radius: 8px;
  font-weight: 600;
  font-size: 14px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  min-width: 140px;
  text-align: center;
}

.box.neural {
  background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
}

.box.success {
  background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
}

.diamond {
  background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);
  color: #333;
  padding: 12px 16px;
  border-radius: 50%;
  font-weight: 600;
  font-size: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  min-width: 120px;
  text-align: center;
  transform: rotate(45deg);
}

.diamond span {
  transform: rotate(-45deg);
  display: block;
}

.arrow {
  font-size: 24px;
  color: #667eea;
  margin: 4px 0;
  font-weight: bold;
}

.decision-arrows {
  display: flex;
  gap: 40px;
  margin-top: 8px;
}

.arrow-left, .arrow-down {
  font-size: 14px;
  color: #667eea;
  font-weight: 600;
}

.applications-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
  margin: 20px 0;
}

.app-category {
  background: white;
  border-radius: 12px;
  padding: 16px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  border-left: 4px solid;
}

.app-category.vision {
  border-left-color: #ff6b6b;
  background: linear-gradient(135deg, #fff5f5 0%, #ffe8e8 100%);
}

.app-category.nlp {
  border-left-color: #4ecdc4;
  background: linear-gradient(135deg, #f0fdfc 0%, #e6fffa 100%);
}

.app-category.rl {
  border-left-color: #45b7d1;
  background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
}

.app-category.gen {
  border-left-color: #f9ca24;
  background: linear-gradient(135deg, #fffbeb 0%, #fef3c7 100%);
}

.app-category h4 {
  margin: 0 0 12px 0;
  font-size: 16px;
  font-weight: 700;
  color: #333;
}

.app-category ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

.app-category li {
  padding: 4px 0;
  font-size: 13px;
  color: #555;
  position: relative;
  padding-left: 16px;
}

.app-category li:before {
  content: "•";
  position: absolute;
  left: 0;
  color: #667eea;
  font-weight: bold;
}
</style>