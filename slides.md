---
# Available themes: default, seriph, apple, bricks, dracula, geist, light, minimal, nord, purplin, shibainu, unicorn
theme: default
# Custom background for a tech/AI feel
background: https://images.unsplash.com/photo-1518709268805-4e9042af2176?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80
# Apply classes to current slide
class: 'text-center'
# Syntax highlighter
highlighter: shiki
# Show line numbers in code blocks
lineNumbers: true
# Slide information
info: |
  ## Deep Learning Overview
  A comprehensive introduction to deep learning concepts and applications.
  
  Modern AI presentation template.
# Persist drawings
drawings:
  persist: false
# Custom fonts
fonts:
  sans: 'Inter'
  serif: 'Inter'
  mono: 'Fira Code'
---

# Deep Learning Revolution
## Transforming AI with Neural Networks

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-4 py-2 rounded-lg cursor-pointer bg-blue-500 bg-opacity-20 hover:bg-opacity-30 transition-all duration-300">
    Start Journey <carbon:arrow-right class="inline ml-2"/>
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

<style>
h1 {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 3.5rem !important;
  font-weight: 800;
}

h2 {
  color: rgba(255, 255, 255, 0.8);
  font-weight: 400;
  font-size: 1.5rem;
  margin-top: 1rem;
}
</style>

---
layout: intro
class: text-left
---

# What is Deep Learning?

<div class="grid grid-cols-2 gap-12 mt-8">

<div>

## Core Concepts

<v-clicks>

- 🧠 **Neural Networks**  
  Multi-layered artificial neurons

- 📊 **Pattern Recognition**  
  Automatic complex pattern discovery

- 🔄 **Backpropagation**  
  Weight optimization algorithm

- 🎯 **Feature Learning**  
  Automatic representation extraction

- ⚡ **GPU Acceleration**  
  Massive parallel processing

- 🌐 **Universal Approximation**  
  Can model any continuous function

</v-clicks>

</div>

<div>

## Key Advantages

<v-clicks>

- **Automatic Feature Engineering**  
  No manual feature extraction needed

- **Scalable Performance**  
  Improves with more data

- **Transfer Learning**  
  Reuse pre-trained models

- **End-to-End Learning**  
  Direct input-to-output mapping

- **State-of-the-Art Results**  
  Leading performance across domains

</v-clicks>

</div>

</div>

<style>
h1 {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 2.5rem;
  font-weight: 700;
}

h2 {
  color: #4a5568;
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 1.5rem;
}

li {
  margin-bottom: 1rem;
  font-size: 1rem;
}

strong {
  color: #2d3748;
  font-weight: 600;
}
</style>

---
layout: center
class: text-center
---

# Deep Learning Ecosystem

<div class="grid grid-cols-2 gap-16 mt-12">

<div>

## 🔄 Development Process

<div class="text-center space-y-4">

<v-clicks>

**1. Data Collection** 📊  
*Gather & preprocess datasets*

↓

**2. Model Design** 🏗️  
*Architecture selection*

↓

**3. Training** 🎯  
*Optimize parameters*

↓

**4. Evaluation** 📈  
*Test performance*

↓

**5. Deployment** 🚀  
*Production ready*

</v-clicks>

</div>

</div>

<div>

## 🚀 Applications

<v-clicks>

**👁️ Computer Vision**
- Image Classification
- Object Detection  
- Medical Imaging
- Autonomous Driving

**💬 Natural Language**
- ChatGPT & LLMs
- Machine Translation
- Sentiment Analysis
- Text Generation

**🎵 Audio Processing**
- Speech Recognition
- Music Generation
- Voice Synthesis
- Audio Classification

**🎮 Reinforcement Learning**
- Game AI (AlphaGo)
- Robotics Control
- Trading Systems
- Resource Optimization

</v-clicks>

</div>

</div>

<div class="mt-12">
  <h3 class="text-2xl font-bold mb-4">Popular Frameworks</h3>
  <div class="flex gap-4 justify-center">
    <a href="https://tensorflow.org" class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600">TensorFlow</a>
    <a href="https://pytorch.org" class="px-4 py-2 bg-orange-500 text-white rounded hover:bg-orange-600">PyTorch</a>
    <a href="https://keras.io" class="px-4 py-2 bg-red-500 text-white rounded hover:bg-red-600">Keras</a>
    <a href="https://huggingface.co" class="px-4 py-2 bg-yellow-500 text-white rounded hover:bg-yellow-600">Hugging Face</a>
  </div>
</div>

<style>
h1 {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 3rem;
  font-weight: 700;
}

</style>