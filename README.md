# Text-Summarization-NLP-Project

## Dataset Card for SAMSum Corpus
### Dataset Summary
The SAMSum dataset contains about 16k messenger-like conversations with summaries. Conversations were created and written down by linguists fluent in English. Linguists were asked to create conversations similar to those they write on a daily basis, reflecting the proportion of topics of their real-life messenger convesations. The style and register are diversified - conversations could be informal, semi-formal or formal, they may contain slang words, emoticons and typos. Then, the conversations were annotated with summaries. It was assumed that summaries should be a concise brief of what people talked about in the conversation in third person. The SAMSum dataset was prepared by Samsung R&D Institute Poland and is distributed for research purposes (non-commercial licence: CC BY-NC-ND 4.0).


### Workflows
1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the pipeline
7. update the main.py
8. update the app.py


### Text Summarization NLP Project

Project Overview
This project implements an automatic text summarization tool using Natural Language Processing (NLP) techniques. Text summarization helps generate concise summaries of large texts, making it easier for users to extract essential information quickly. This project explores different summarization techniques, including extractive and abstractive methods, to produce effective and accurate summaries.

Table of Contents
Motivation
Dataset
Technologies Used
Installation
Usage
Summarization Techniques
Results
Future Enhancements
Contributors
License
Motivation
With the ever-growing amount of text data available, it’s challenging to go through lengthy documents or articles. Automatic text summarization can help users quickly understand the key points of a document, which is valuable in fields like journalism, research, and business intelligence. This project aims to demonstrate the power of NLP in condensing information without losing the essential content.

Dataset
This project works with a dataset of long-form text documents, which may include articles, research papers, or other large text sources. The dataset is either sourced from publicly available text data or custom-generated for educational purposes.

Preprocessing Steps
Tokenization
Stopword removal
Text cleaning (punctuation and noise removal)
Sentence segmentation for extractive summarization
Technologies Used
Python 3.8+
NLTK: Text preprocessing and tokenization
spaCy: Advanced NLP processing
Gensim: Extractive summarization
Transformers (Hugging Face): Abstractive summarization using transformer models (e.g., BART, T5)
Flask: Simple web interface for summarization
Installation
To set up this project locally, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/Om700-create/Text-Summarization-NLP-Project.git
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Run the Flask application:

bash
Copy code
python app.py
Usage
Extractive Summarization: Selects key sentences from the original text to form a summary. This approach retains original sentences, making it more factual.
Abstractive Summarization: Generates new sentences that capture the core meaning, similar to how a human would summarize text. Uses transformer-based models such as BART or T5.
Web Interface: Users can input text or upload documents through a simple web interface and receive a summary instantly.
Summarization Techniques
This project implements both extractive and abstractive summarization techniques:

Extractive Summarization: Uses techniques such as frequency-based methods and TextRank (via Gensim) to select the most representative sentences from the text.

Abstractive Summarization: Utilizes advanced NLP models from the Hugging Face Transformers library, including:

BART: A transformer model fine-tuned for summarization tasks
T5: A versatile transformer model that can generate high-quality abstractive summaries
Each model is evaluated based on the quality and readability of generated summaries.

Results
The project achieved the following results on test documents:

Extractive Summarization: Maintained factual accuracy with an average compression ratio of XX%.
Abstractive Summarization: Produced human-like summaries with coherence scores of XX%, and fluency scores of XX%.
The results indicate that both techniques have unique strengths, with extractive summaries being more precise and abstractive summaries offering better readability.

Future Enhancements
Some potential areas for improvement include:

Fine-tuning Models: Further fine-tuning of BART and T5 models on domain-specific datasets.
Hybrid Summarization: Combining extractive and abstractive approaches for better accuracy and coherence.
Multi-Document Summarization: Extending the project to handle multiple documents and summarize across them.
Contributors
Narayan Bhandari
License
This project is licensed under the MIT License. See the LICENSE file for more details.

