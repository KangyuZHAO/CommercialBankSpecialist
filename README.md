# CommercialBankSpecialist

- Data Sources: The German Credit Dataset from the UCI Machine Learning Repository and a synthetic credit card policy document in English, Chinese, French, and German.
- Embedding and Retrieval: The sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2 model generates embeddings for documents, which are indexed using FAISS for efficient similarity search.
- Generation Model: A fine-tuned curiousily/Llama-3-8B-Instruct-Finance-RAG model, loaded in 4-bit quantization to optimize memory usage, generates responses.
- Translation: Helsinki-NLP translation pipelines (opus-mt-en-es and opus-mt-en-de) enable multilingual responses in Spanish and German.
- User Interface: A Gradio-based interface supports text queries, file uploads (txt, pdf, csv), and chart generation for data visualization.
