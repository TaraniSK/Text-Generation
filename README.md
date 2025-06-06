
# 🔤 Character-Level Text Generation using RNN/LSTM

This project implements a character-level text generation model using PyTorch. It learns from Shakespearean dialogue data to generate new text one character at a time using either RNN or LSTM architectures.

---

## 📁 Dataset

The model uses a dataset of Shakespearean dialogues loaded from a CSV file (e.g., `Shakespeare_data.csv`). Only the `PlayerLine` column is used to train the model.

---

## 🧠 Model Architecture

- **Embedding Layer**: Converts characters to dense vectors.
- **RNN/LSTM**: Learns temporal patterns from sequences of characters.
- **Fully Connected Layer**: Maps hidden states to output character probabilities.

You can switch between RNN and LSTM using the `use_lstm` flag.

---

## ⚙️ Configuration

```python
sequence_length = 100
embedding_dim = 128
hidden_size = 256
num_layers = 2
dropout_rate = 0.2
learning_rate = 0.003
batch_size = 64
num_epochs = 20
use_lstm = True
````

---

## 🚀 How It Works

1. **Data Loading**: Load and clean character sequences from the CSV file.
2. **Dataset & Dataloader**: Prepare sequences of length 100 and next-character targets.
3. **Model Training**: Train using cross-entropy loss and Adam optimizer.
4. **Text Generation**: Start from a user-provided string and generate new characters.

---

## 📈 Evaluation

* Training loss is recorded and plotted across epochs.
* Text generation uses **temperature-based sampling** to control randomness.

---

## 📊 Optional Metrics (Available to Extend)

* **BLEU Score**: Can be used to compare generated vs. reference text.
* **Confusion Matrix**: Applicable if doing character-level classification.

---

## 📷 Sample Output

```
Input: "king "
Generated: "king and the lord hath he is the heart and he shall be the love..."
```

---

## 🛠️ Dependencies

* Python 3.x
* PyTorch
* NumPy
* Pandas
* Matplotlib
* NLTK
* scikit-learn

Install using:

```bash
pip install torch numpy pandas matplotlib nltk scikit-learn
```

---

## 📌 To Do

* [ ] Add BLEU score evaluation
* [ ] Add character-level confusion matrix
* [ ] Implement saving and loading models
* [ ] Add UI with Gradio or Streamlit

---

## 📜 License

This project is under the MIT License. Feel free to fork and build on top of it!

---

## ✨ Acknowledgment

Based on Shakespearean plays dataset and inspired by sequence modeling techniques in NLP.

```

---

Would you like me to generate a downloadable `.md` file version for you?
```
