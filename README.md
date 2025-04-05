Project Title: Document Similarity Detection System
Description:
This project is designed to detect the similarity between documents using two core algorithms: Cosine Similarity for word-based comparison, and Latent Semantic Analysis (LSA) for semantic (meaning-based) similarity. The system is modular and scalable, processing multiple documents and comparing them to identify content overlap both at the surface level (words) and deeper conceptual level (meaning).

Modules Overview:
Preprocessing Module:

Cleans and tokenizes the input documents.

Removes stop words, punctuation, and applies stemming/lemmatization to prepare raw textual data for analysis.

Bag of Words (BoW):

Creates a frequency-based word representation of documents.

Used for simple content matching by counting the occurrences of words.

Term Frequency–Inverse Document Frequency (TF-IDF):

Calculates the importance of words in each document relative to the entire dataset.

Helps in weighing down common terms and highlighting distinctive ones.

Document Calculator:

Performs vector multiplication of TF and IDF values.

Converts textual data into numerical vectors for similarity comparison.

Cosine Similarity Module:

Compares the vectors generated from each document.

Measures angle-based similarity between documents focusing on word content.

Latent Semantic Analysis (LSA):

Applies dimensionality reduction to capture hidden relationships between terms and documents.

Compares documents based on their underlying meaning rather than just word usage.

Working Mechanism:
The first three modules (Preprocessing, BoW, TF-IDF) operate independently on each document to convert them into structured data.

The last three modules (Document Calculator, Cosine, LSA) work together to compare all documents in the dataset and compute similarity scores.

Users can upload multiple files, and the system will return similarity metrics both by word usage and semantic meaning.

Technologies Used:
Programming Language: Python

Libraries: NumPy, SciPy, scikit-learn, NLTK, Pandas

Algorithms: Cosine Similarity, LSA (using SVD)

