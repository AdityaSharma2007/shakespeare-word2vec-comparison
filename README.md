Comparative Analysis of CBOW and Skip-Gram Word Embeddings on Shakespeare Corpus

# shakespeare-word2vec-comparison
Comparative study of CBOW and Skip-gram Word2Vec models trained on Shakespeare corpus with semantic similarity analysis and PCA-based visualization.


📌 Project Overview

This project explores and compares two Word2Vec architectures — CBOW (Continuous Bag of Words) and Skip-gram — trained on The Complete Works of William Shakespeare.

The objective is to analyze semantic relationships between words, evaluate embedding quality, and visualize high-dimensional word vectors using PCA.

🧠 Motivation

Word embeddings are fundamental to modern NLP systems.
This project aims to understand:

How CBOW and Skip-gram differ in learning semantics

How dataset size influences embedding quality

How contextual similarity emerges from literature text

⚙️ Methodology
1️⃣ Data Preprocessing

Text files loaded from Shakespeare corpus

Sentence tokenization using NLTK

Tokenization using gensim.simple_preprocess

Stopword removal

Minimum frequency filtering (min_count=2)

2️⃣ Word2Vec Training

Two models were trained:

Model	Architecture	Vector Size	Window	Epochs
CBOW	sg=0	200	10	10
Skip-gram	sg=1	200	10	10
3️⃣ Evaluation

Most similar words analysis

Semantic similarity scoring

Analogy testing

PCA dimensionality reduction

3D embedding visualization using Plotly

📊 Key Observations

CBOW produced stronger semantic clustering for frequent thematic words.

Similarity score (king–queen):

CBOW: 0.73

Skip-gram: 0.44

Emotional and royal vocabulary formed clear semantic clusters.

PCA visualization confirmed contextual grouping.

📈 Example Output

Most similar to "king" (CBOW):

henry, england, france, prince, edward, richard, heir, realm

Most similar to "death":

grave, life, dead, body, buried
🛠️ Technologies Used

Python

Gensim

NLTK

Scikit-learn

Plotly

NumPy

🚀 Future Improvements

Hyperparameter tuning (window size, epochs)

Genre-specific embedding training

Quantitative embedding evaluation metrics

t-SNE visualization comparison

👨‍💻 Author

Aditya Sharma
B.Tech Computer Science Engineering (AI-focused)
Exploring NLP and Machine Learning
