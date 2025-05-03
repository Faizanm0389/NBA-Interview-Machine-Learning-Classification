# 🏀 NBA Interview - NLP Classification Model

This project performs **multi-label text classification** on NBA and WNBA post-game interview responses. The goal is to classify each quote by:
- **Sentiment**: Positive or Negative
- **Focus**: Team or Individual

We fine-tuned a transformer-based model (DistilBERT) to predict these two labels from interview transcripts, and compared its performance with traditional machine learning approaches.

---

## 📁 Dataset

The dataset was sourced from [asapsports.com](https://www.asapsports.com/), consisting of interview quotes from:
- NBA & WNBA Finals
- NBA & WNBA Drafts

Each quote is labeled along two binary axes:
- `Positive`, `Negative` (one is 1, the other blank)
- `Team`, `Individual` (one is 1, the other blank)

### Sample Format:
```csv
quote,Positive,Negative,Team,Individual
"We believe in each other and have to protect home court.",1,,1,
"She means everything to me. She's been incredible.",1,,,1
