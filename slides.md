---
# Available themes: default, seriph, apple, bricks, dracula, geist, light, minimal, nord, purplin, shibainu, unicorn
theme: seriph
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

<div class="process-flow">
  <div class="step-container">
    <div class="step start">
      <div class="step-number">1</div>
      <div class="step-content">
        <h4>Data Collection</h4>
        <p>Gather & preprocess datasets</p>
      </div>
    </div>
    
    <div class="flow-arrow">↓</div>
    
    <div class="step">
      <div class="step-number">2</div>
      <div class="step-content">
        <h4>Model Design</h4>
        <p>Architecture selection</p>
      </div>
    </div>
    
    <div class="flow-arrow">↓</div>
    
    <div class="step">
      <div class="step-number">3</div>
      <div class="step-content">
        <h4>Training</h4>
        <p>Optimize parameters</p>
      </div>
    </div>
    
    <div class="flow-arrow">↓</div>
    
    <div class="step">
      <div class="step-number">4</div>
      <div class="step-content">
        <h4>Evaluation</h4>
        <p>Test performance</p>
      </div>
    </div>
    
    <div class="decision-point">
      <div class="diamond">
        <span>Good Results?</span>
      </div>
      <div class="decision-arrows">
        <div class="arrow-no">← No (Iterate)</div>
        <div class="arrow-yes">↓ Yes</div>
      </div>
    </div>
    
    <div class="step final">
      <div class="step-number">5</div>
      <div class="step-content">
        <h4>Deployment</h4>
        <p>Production ready</p>
      </div>
    </div>
  </div>
</div>

</div>

<div>

## 🚀 Applications

<div class="applications">
  <div class="app-card vision">
    <div class="app-icon">👁️</div>
    <h4>Computer Vision</h4>
    <ul>
      <li>Image Classification</li>
      <li>Object Detection</li>
      <li>Medical Imaging</li>
      <li>Autonomous Driving</li>
    </ul>
  </div>
  
  <div class="app-card nlp">
    <div class="app-icon">💬</div>
    <h4>Natural Language</h4>
    <ul>
      <li>ChatGPT & LLMs</li>
      <li>Machine Translation</li>
      <li>Sentiment Analysis</li>
      <li>Text Generation</li>
    </ul>
  </div>
  
  <div class="app-card audio">
    <div class="app-icon">🎵</div>
    <h4>Audio Processing</h4>
    <ul>
      <li>Speech Recognition</li>
      <li>Music Generation</li>
      <li>Voice Synthesis</li>
      <li>Audio Classification</li>
    </ul>
  </div>
  
  <div class="app-card rl">
    <div class="app-icon">🎮</div>
    <h4>Reinforcement Learning</h4>
    <ul>
      <li>Game AI (AlphaGo)</li>
      <li>Robotics Control</li>
      <li>Trading Systems</li>
      <li>Resource Optimization</li>
    </ul>
  </div>
</div>

</div>

</div>

<div class="mt-12">
  <h3 class="text-2xl font-bold mb-4">Popular Frameworks</h3>
  <div class="frameworks">
    <a href="https://tensorflow.org" class="framework-link">TensorFlow</a>
    <a href="https://pytorch.org" class="framework-link">PyTorch</a>
    <a href="https://keras.io" class="framework-link">Keras</a>
    <a href="https://huggingface.co" class="framework-link">Hugging Face</a>
  </div>
</div>

<style>
.process-flow {
  max-width: 300px;
  margin: 0 auto;
}

.step-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 12px;
}

.step {
  display: flex;
  align-items: center;
  gap: 16px;
  background: white;
  padding: 16px 20px;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  width: 100%;
  transition: transform 0.2s ease;
}

.step:hover {
  transform: translateY(-2px);
}

.step.start {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
}

.step.final {
  background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
  color: white;
}

.step-number {
  background: rgba(255,255,255,0.2);
  color: white;
  width: 32px;
  height: 32px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  font-size: 14px;
}

.step:not(.start):not(.final) .step-number {
  background: #667eea;
  color: white;
}

.step-content h4 {
  margin: 0 0 4px 0;
  font-size: 16px;
  font-weight: 600;
}

.step-content p {
  margin: 0;
  font-size: 12px;
  opacity: 0.8;
}

.flow-arrow {
  font-size: 24px;
  color: #667eea;
  font-weight: bold;
}

.decision-point {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
}

.diamond {
  background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);
  color: #333;
  padding: 16px;
  border-radius: 8px;
  font-weight: 600;
  font-size: 12px;
  text-align: center;
  transform: rotate(45deg);
  width: 80px;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.diamond span {
  transform: rotate(-45deg);
  line-height: 1.2;
}

.decision-arrows {
  display: flex;
  gap: 40px;
  font-size: 12px;
  font-weight: 600;
  color: #667eea;
}

.applications {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
  max-width: 500px;
}

.app-card {
  background: white;
  border-radius: 12px;
  padding: 20px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: transform 0.2s ease;
}

.app-card:hover {
  transform: translateY(-4px);
}

.app-card.vision {
  border-left: 4px solid #ff6b6b;
}

.app-card.nlp {
  border-left: 4px solid #4ecdc4;
}

.app-card.audio {
  border-left: 4px solid #45b7d1;
}

.app-card.rl {
  border-left: 4px solid #f9ca24;
}

.app-icon {
  font-size: 24px;
  margin-bottom: 8px;
}

.app-card h4 {
  margin: 0 0 12px 0;
  font-size: 14px;
  font-weight: 700;
  color: #333;
}

.app-card ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

.app-card li {
  padding: 2px 0;
  font-size: 11px;
  color: #555;
  position: relative;
  padding-left: 12px;
}

.app-card li:before {
  content: "•";
  position: absolute;
  left: 0;
  color: #667eea;
  font-weight: bold;
}

.frameworks {
  display: flex;
  gap: 16px;
  justify-content: center;
  flex-wrap: wrap;
}

.framework-link {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 8px 16px;
  border-radius: 20px;
  text-decoration: none;
  font-weight: 600;
  font-size: 14px;
  transition: transform 0.2s ease;
}

.framework-link:hover {
  transform: translateY(-2px);
}

h1 {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 3rem;
  font-weight: 700;
}

h3 {
  color: #4a5568;
}
</style>