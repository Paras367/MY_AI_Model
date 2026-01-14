# 🧠 MY_AI_MODEL — Browser-Based AI Spam Detector

A **fully client-side AI** that runs 100% in your browser — no server, no API keys, no cost.  
Trained to detect spam vs. legitimate messages using TensorFlow.js.

> 🔥 **Live Demo**: [https://paras367.github.io/MY_AI_Model](https://paras367.github.io/MY_AI_Model) 


---

## ✨ Features
- ✅ **Zero backend** — all inference happens in-browser
- ✅ **Privacy-first** — your messages never leave your device
- ✅ **Lightweight** — model < 100 KB
- ✅ **Single HTML file** — easy to embed or share
- ✅ Trained on clear spam/ham examples for high accuracy

---

## 🚀 Try It Now
1. Open the [live demo](https://paras367.github.io/MY_AI_Model)
2. Type a message like:
   - `"Winner! Claim your prize now!"` → 🚨 **SPAM**
   - `"Hi, can we reschedule the meeting?"` → ✅ **NOT SPAM**

---

## 📁 Repository Structure
MY_AI_MODEL/
├── index.html     # Single-file frontend (HTML + CSS + JS)
├── config.json    # Vocabulary + input dimension
├── README.md
└── tfjs_model/    # TensorFlow.js model files
├── model.json
└── group1-shard1of1.bin

---

## ⚙️ How It Works
1. **Training**:  
   - Model trained in [Google Colab](https://colab.research.google.com/) using a custom dataset
   - Architecture: Dense neural network (input → hidden → sigmoid output)
   - Exported as **SavedModel**, then converted to **TensorFlow.js**

2. **Frontend**:  
   - Loads `config.json` to map words → indices
   - Encodes input text into a fixed-length vector (matches training)
   - Runs inference using `@tensorflow/tfjs`
   - Displays confidence score in real time

3. **No external dependencies** — everything is self-contained!

---

## 🌐 Hosting
This repo is ready for **GitHub Pages**:
1. Go to **Settings > Pages**
2. Set **Branch: `main`**, **Folder: `/root`**
3. Visit `https://paras367.github.io/MY_AI_Model`

---

## 📜 License
MIT License — free to use, modify, and distribute.

---

## 🙌 Made by
[PARAS DHIMAN(CyberVex)] • [Paras367](https://paras367.github.io/)

> Built with ❤️ using TensorFlow, TensorFlow.js, and pure HTML/CSS/JS.
