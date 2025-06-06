# ✂️ Semantic & Rule-Based Text Chunking Playground

Welcome to the **Chunking Techniques Exploration** notebook — your all-in-one lab for experimenting with SOTA and classical methods for splitting long texts into meaningful chunks.

---

## 🚀 What's Inside

| Method                  | Type            | Description                                                                 |
|------------------------|-----------------|-----------------------------------------------------------------------------|
| `RegexSplitter`        | Rule-Based      | Split text using custom regular expressions (e.g., `Article \d+`)          |
| `StatisticalChunker`<br>`Custom Greg Kamradt's chunker`   | Semantic        | Uses dynamic thresholds on embedding similarity (SOTA by SemanticRouter)   |
| `ConsecutiveChunker`   | Semantic        | Compares sentence-wise chunk similarity and splits adaptively              |
| `CumulativeChunker`    | Semantic        | Accumulates context and splits when similarity with previous chunk drops   |

---


## 💡 Tips

- Use `RegexSplitter` when structure is clear (e.g. legal documents, manuals).
- Use `StatisticalChunker` for general-purpose semantic chunking.
- Use `CumulativeChunker` when long-term context is important (e.g., narratives).
- Use `ConsecutiveChunker` when you want to detect subtle topic shifts sentence by sentence, ideal for structured but evolving content like tutorials, conversations, or Q&A.
- Combine rule-based pre-chunking with semantic refinement for best results.

---

## 🛠️ Dependencies
Recommended to use `python3.11`\
Install via poetry:
```bash
pip install poetry
poetry init 
poetry install
```

Install via pip:

```bash
pip install -r requirements.txt
```

---


### 👋 Contacts

📨 - [fivashchenko0308@gmail.com](mailto:fivashchenko0308@gmail.com)  
📲 - [Telegram](https://t.me/IvashchenkoF)