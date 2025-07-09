---
# Available themes: default, seriph, apple, bricks, dracula, geist, light, minimal, nord, purplin, shibainu, unicorn
theme: seriph
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
# Persist drawings
drawings:
  persist: false
---

# Deep Learning Revolution
## Transforming AI with Neural Networks

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-6 py-3 rounded-lg cursor-pointer bg-blue-600 text-white hover:bg-blue-700 transition-all duration-300 font-semibold">
    開始探索 <carbon:arrow-right class="inline ml-2"/>
  </span>
</div>

---
layout: default
---

# 什麼是深度學習？

<div class="grid grid-cols-2 gap-8 mt-8">

<div>

## 核心概念

- 🧠 **神經網路**  
  多層人工神經元結構

- 📊 **模式識別**  
  自動發現複雜模式

- 🔄 **反向傳播**  
  權重優化演算法

- 🎯 **特徵學習**  
  自動提取表示特徵

- ⚡ **GPU 加速**  
  大規模平行處理

</div>

<div>

## 主要優勢

- **自動特徵工程**  
  無需手動特徵提取

- **可擴展性能**  
  隨數據增加而改善

- **遷移學習**  
  重複使用預訓練模型

- **端到端學習**  
  直接輸入到輸出映射

- **最先進結果**  
  各領域領先性能

</div>

</div>

---
layout: center
class: text-center
---

# 深度學習開發流程

<div class="flowchart-container">

```mermaid
flowchart TD
    A[數據收集<br/>Data Collection] --> B[數據預處理<br/>Data Preprocessing]
    B --> C[模型設計<br/>Model Design]
    C --> D[模型訓練<br/>Model Training]
    D --> E[模型評估<br/>Model Evaluation]
    E --> F{性能滿足要求?<br/>Performance OK?}
    F -->|否 No| C
    F -->|是 Yes| G[模型部署<br/>Deployment]
    G --> H[監控維護<br/>Monitoring]
    
    style A fill:#e1f5fe
    style B fill:#f3e5f5
    style C fill:#fff3e0
    style D fill:#e8f5e8
    style E fill:#fff8e1
    style F fill:#ffebee
    style G fill:#e0f2f1
    style H fill:#f1f8e9
```

</div>

---
layout: two-cols
---

# 應用領域

## 🖼️ 電腦視覺
- 圖像分類
- 物體檢測
- 醫學影像分析
- 自動駕駛

## 💬 自然語言處理
- ChatGPT 與大語言模型
- 機器翻譯
- 情感分析
- 文本生成

::right::

## 🎵 音訊處理
- 語音識別
- 音樂生成
- 語音合成
- 音訊分類

## 🎮 強化學習
- 遊戲 AI (AlphaGo)
- 機器人控制
- 交易系統
- 資源優化

---
layout: center
class: text-center
---

# 熱門深度學習框架

<div class="frameworks-grid">

<div class="framework-card tensorflow">
  <img src="https://www.tensorflow.org/images/tf_logo_social.png" alt="TensorFlow" class="framework-logo">
  <h3>TensorFlow</h3>
  <p>Google 開發的開源機器學習平台</p>
</div>

<div class="framework-card pytorch">
  <img src="https://pytorch.org/assets/images/pytorch-logo.png" alt="PyTorch" class="framework-logo">
  <h3>PyTorch</h3>
  <p>Facebook 開發的動態神經網路框架</p>
</div>

<div class="framework-card keras">
  <div class="framework-icon">🔥</div>
  <h3>Keras</h3>
  <p>高級神經網路 API</p>
</div>

<div class="framework-card huggingface">
  <div class="framework-icon">🤗</div>
  <h3>Hugging Face</h3>
  <p>自然語言處理模型庫</p>
</div>

</div>

<style>
.frameworks-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2rem;
  max-width: 800px;
  margin: 2rem auto;
}

.framework-card {
  background: white;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
  border: 2px solid transparent;
}

.framework-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.15);
}

.framework-card.tensorflow {
  border-color: #ff6f00;
}

.framework-card.pytorch {
  border-color: #ee4c2c;
}

.framework-card.keras {
  border-color: #d00000;
}

.framework-card.huggingface {
  border-color: #ff9d00;
}

.framework-logo {
  width: 60px;
  height: 60px;
  object-fit: contain;
  margin: 0 auto 1rem;
  display: block;
}

.framework-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.framework-card h3 {
  margin: 0 0 0.5rem 0;
  font-size: 1.5rem;
  font-weight: 600;
}

.framework-card p {
  margin: 0;
  color: #666;
  font-size: 0.9rem;
}

.flowchart-container {
  background: white;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  margin: 2rem auto;
  max-width: 900px;
}
</style>

---
layout: center
class: text-center
---

# 深度學習的未來

<div class="grid grid-cols-3 gap-8 mt-8">

<div class="future-card">
  <div class="future-icon">🚀</div>
  <h3>更強大的模型</h3>
  <p>GPT-4、Claude 等大型語言模型持續進化</p>
</div>

<div class="future-card">
  <div class="future-icon">⚡</div>
  <h3>更高效的計算</h3>
  <p>專用 AI 晶片和量子計算的發展</p>
</div>

<div class="future-card">
  <div class="future-icon">🌍</div>
  <h3>更廣泛的應用</h3>
  <p>從科學研究到日常生活的全面滲透</p>
</div>

</div>

<div class="mt-12">
  <h2 class="text-2xl font-bold mb-4">謝謝聆聽！</h2>
  <p class="text-lg text-gray-600">Questions & Discussion</p>
</div>

<style>
.future-card {
  background: white;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.future-card:hover {
  transform: translateY(-4px);
}

.future-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.future-card h3 {
  margin: 0 0 1rem 0;
  font-size: 1.25rem;
  font-weight: 600;
}

.future-card p {
  margin: 0;
  color: #666;
  font-size: 0.9rem;
  line-height: 1.5;
}
</style>