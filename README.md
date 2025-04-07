# 🧠 Word-Level GPT Language Model

This project implements a simplified GPT-style autoregressive language model trained on the **Tiny Shakespeare** dataset using **word-level tokenization**.

---

## 🚀 Features

- ✅ Word-level vocabulary creation from raw text  
- ✅ Custom encoding/decoding functions for word ↔ index  
- ✅ PyTorch-based GPT model implementation from scratch  
- ✅ Positional embeddings + causal self-attention  
- ✅ Transformer block with multi-head attention and feed-forward layers  
- ✅ Text generation using sampling from softmax output  
- ✅ Training and validation loss monitoring  
- ✅ Support for CPU and GPU (CUDA)

---

## 📂 Project Structure

```
word-gpt/
├── gpt_model.py                # GPT model architecture (attention, transformer blocks)
├── train_gpt.py                # Training loop and generation logic
├── tokenizer_utils.py          # Word-level vocabulary, encode/decode utilities
├── README.md                   # Project overview and setup
```

---

## 📊 Dataset

- **Source**: [Tiny Shakespeare dataset](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)  
- **Tokenization**: Word-based (via `.split()`)

---

## ⚙️ Hyperparameters

- `block_size`: 32 (context window size)  
- `batch_size`: 16  
- `embed_dim`: 128  
- `n_layers`: 4  
- `num_heads`: 4  
- `ffw_hidden_dim`: 256  
- `learning_rate`: 3e-4  
- `max_steps`: 1000

---

## 🔧 How to Run

```bash
# Install PyTorch and dependencies
pip install torch

# Run training script
python train_gpt.py

# Sample generation
python generate_text.py
```

---

## 🧪 Sample Output

```text
Prompt: House  
Generated: House of the day of the world to be the same to be the most of the man and
```

---

## 📈 Future Improvements

- Add temperature/top-k sampling for more diverse generation  
- Switch to subword-level encoding (BPE)  
- Add CLI or notebook interface for prompt-based generation  

---

## ❤️ Acknowledgments

- Inspired by [Andrej Karpathy's minGPT](https://github.com/karpathy/minGPT)  
- Built from scratch using PyTorch

---

## 📜 License

This project is open-source and licensed under the MIT License.
