## 📈 Final Results – Spelling Correction System

### 🔍 Overview
The spelling correction system was designed as a **hybrid framework** combining:
- **Levenshtein Edit Distance** for candidate generation  
- **Noisy Channel Model** for probabilistic ranking  
- **Bigram Language Model** for contextual validation  

An interactive **Gradio interface** was implemented to highlight errors (red underline for non-word, blue underline for real-word) and provide one‑click correction suggestions.

---

### 📊 Performance
- **Non-word detection**: Successfully flagged typos such as *“stk” → “stock”* and *“acording” → “according”*.  
- **Real-word detection**: Correctly identified contextual errors, e.g., *“peace of the company” → “piece of the company”*.  
- **Efficiency**: Optimizations (length-window pruning, edit distance threshold, probability cut-offs) ensured **real-time response** for inputs up to 500 characters.  

---

### 📝 Strengths
- High domain-specific accuracy using the **AG News Business corpus**  
- Dual-layer detection (lexical + contextual) improved robustness  
- Real-time performance achieved through algorithmic optimizations  
- User-friendly interface with error highlighting and interactive correction workflow  

---

### ⚠️ Limitations
- Vocabulary restricted to the AG News corpus; cannot handle unseen brand names or technical jargon  
- Bigram model affected by data sparsity, occasionally producing false positives for rare word sequences  

---

### ✅ Conclusion
The hybrid Bayesian–Levenshtein spelling correction system achieved **strong accuracy and responsiveness** in business-domain text. While effective for domain-specific tasks, future improvements could include:
- Expanding the corpus for broader vocabulary coverage  
- Incorporating neural-based N-gram or transformer models to better capture long-range dependencies  

