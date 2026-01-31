# Embedding Retrieval Demo

An interactive **Streamlit** demo for semantic retrieval / prototype classification.  
Given user-defined categories and an input sentence, the app converts both the sentence and each category into embeddings using multiple models, computes similarity scores, and visualizes the results.

## Features

- **Multi-model comparison**: Compare results from **GloVe 50d**, **SentenceTransformer 384d**, and **OpenAI text-embedding-3-small / text-embedding-3-large** on the same input.
- **Custom categories**: Users can enter arbitrary categories (space-separated) and instantly retrieve the closest category for the input text.
- **Similarity visualization**: Displays a pie chart of normalized similarity distribution across categories, plus a table summarizing each model’s **Top Category** and **Confidence Score**.
- **Lightweight retrieval logic**: Uses **cosine similarity** (with `exp(cos)` to ensure positive scores) to implement a minimal semantic retrieval / prototype classification pipeline.
