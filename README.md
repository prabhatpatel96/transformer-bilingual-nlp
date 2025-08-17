# Transformer-Based Bilingual Text Generation (English ↔ Hindi)

🚀 **Self Project** — Implementation of a custom Transformer model from scratch for **English–Hindi translation**, built without high-level Transformer libraries.
**BLEU 27.8 and METEOR 0.41**
## 📌 Project Overview
This project implements a Transformer architecture **entirely from scratch** in PyTorch for bilingual translation between English and Hindi. It is trained on the **IIT Bombay Parallel Corpus** and replicates both forward and backward passes using only PyTorch’s `autograd`, without relying on high-level APIs like `nn.Transformer`.

## ✨ Key Features
- **Custom Transformer Implementation** — Encoder-Decoder architecture coded from scratch.
- **Core Modules** — Multi-Head Attention, Positional Encoding, Layer Normalization.
- **Manual Training Pipeline** — Custom forward/backward pass implementation using `autograd`.
- **Bilingual Support** — Trained on IIT Bombay English–Hindi parallel dataset.
- **High Translation Accuracy** — Demonstrates deep understanding of NLP modeling and training dynamics.

## 🛠️ Tech Stack
- **Language:** Python 3.x
- **Libraries:** PyTorch, NumPy, Pandas
- **Dataset:** IIT Bombay Parallel Corpus
- **Environment:** Cross-platform (Windows / Linux)

## 📂 Project Structure
.
├── config.py # Configuration for training and model parameters
├── dataset.py # Dataset loading and preprocessing pipeline
├── model.py # Transformer model implementation
├── train.py # Training loop with custom forward/backward passes
├── translate.py # Translation inference script
├── requirements.txt # Python dependencies
├── report.pdf # Detailed project report
└── .gitignore # Ignored files and directories


## 📊 Model Architecture
- **Encoder:**
  - Input Embedding + Positional Encoding
  - Multi-Head Self-Attention
  - Feed Forward Network
- **Decoder:**
  - Masked Multi-Head Self-Attention
  - Encoder–Decoder Attention
  - Feed Forward Network
- **Output:** Linear + Softmax for word prediction

## 🚀 Installation & Usage
### 1️⃣ Clone Repository
```bash
git clone https://github.com/prabhatpatel96/transformer-bilingual-nlp.git
cd transformer-bilingual-nlp
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Train the Model
python train.py
4️⃣ Translate Text
python translate.py --text "Hello world" --direction en2hi
📈 Example Translation
Input (English):
I love learning new languages.
Output (Hindi):
मुझे नई भाषाएँ सीखना पसंद है।
