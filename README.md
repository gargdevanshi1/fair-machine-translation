# 🌍 Inclusive Hindi-English Machine Translation  
**Mitigating Gender Bias in MT using Adversarial Learning + Data Augmentation**

This project explores and addresses gender bias in machine translation (MT), specifically for Hindi-English language pairs. While most research focuses on binary gender fairness, our work expands inclusivity by integrating non-binary gender representations through **data augmentation** and **adversarial training** on top of a **pre-trained Marian MT model**.

---

## 🔍 Motivation

Machine translation systems often reflect and amplify gender biases present in training data, reinforcing harmful societal stereotypes. While many existing mitigation techniques address binary gender distinctions, **non-binary and inclusive gender representations** remain largely ignored.

This project aims to:  
- Examine and measure gender bias in a pre-trained Marian MT model  
- Develop a more inclusive MT system by incorporating non-binary representations  
- Evaluate the effectiveness of **adversarial learning** in reducing gender bias  

---

## 💡 Approach

We use a two-fold strategy:
1. **Data Augmentation:** Modify and extend the IIT Bombay English-Hindi Parallel Corpus with explicit gender-based annotations and non-binary-inclusive sentences.
2. **Adversarial Learning:** Incorporate a discriminator network to encourage the encoder to produce gender-neutral representations during translation.

---

## 🛠️ Implementation Steps

✅ Preprocessed the **IIT Bombay English-Hindi Corpus** to normalize formatting and tokenize sentences  
✅ Identified **gender-indicative keywords** in Hindi and English for gender annotation  
✅ Introduced an **adversarial network** into the MT model to discourage learning gendered associations  
✅ Re-trained the MT system on the augmented dataset  
✅ Evaluated translations using BLEU scores, bias metrics, and qualitative comparisons

---

## 📈 Evaluation

- Used controlled gender-specific and gender-neutral test sets to evaluate MT output
- Measured **BLEU score** and **gender bias metrics** pre- and post-mitigation

---

## 📦 Tools & Frameworks

- Language: `Python`, `PyTorch`, `Transformers`
- Pre-trained Model: [`Helsinki-NLP/opus-mt-hi-en`](https://huggingface.co/Helsinki-NLP/opus-mt-hi-en) (MarianMT)
- Libraries: `Hugging Face Transformers`, `Torchtext`, `Fairseq`, `NumPy`, `Pandas`

---

## 🧪 Sample Output

| Source Sentence (Hindi) | Baseline MarianMT Output | Our Model Output |
|-------------------------|--------------------------|------------------|
| वह एक डॉक्टर है।       | He is a doctor.          | They are a doctor. |

---

## 🌐 Broader Impact

By promoting gender inclusivity in translation, this work highlights the **ethical design of NLP systems**. Addressing gender bias is a crucial step in building **responsible AI** systems that treat all identities with fairness and respect.

---

## 📚 Future Work

- Extend beyond Hindi-English to other low-resource languages  
- Explore multilingual gender bias mitigation techniques  
- Incorporate **context-aware transformers** for dynamic gender neutrality

---

## 👩‍💻 Contributors

- **Devanshi Garg**  
  MS in Computer Science, UC San Diego  
  Focus: NLP, Fairness in AI, Deep Learning  
  [LinkedIn](https://linkedin.com/in/garg-devanshi)

---

## 📝 License

This project is intended for research and educational use.
