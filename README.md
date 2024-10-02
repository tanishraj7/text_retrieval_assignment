# text_retrieval_assignment
Task Overview:
The goal of this assignment is to implement a multi-stage text retrieval pipeline for question-answering tasks, incorporating both embedding models and ranking models. You will benchmark different ranking models to assess their impact on retrieval accuracy and understand trade-offs related to model size, accuracy, and performance.

Tasks:
Paper: https://www.arxiv.org/abs/2409.07691
Literature Review and Understanding:
Read the provided paper thoroughly to understand the concepts of multi-stage text retrieval, embedding models, and ranking models.
Summarize the key points, focusing on how ranking models enhance retrieval accuracy in Q&A systems.

Dataset Preparation:
Use publicly available Q&A datasets from the BEIR benchmark, such as Natural Questions (NQ), HotpotQA, and FiQA.
Ensure that the datasets are preprocessed appropriately (e.g., chunked into passages, tokenized).

Implement the Retrieval Pipeline:
Stage 1 - Candidate Retrieval:
Select at least two embedding models (one small and one large) that are commercially usable (e.g., sentence-transformers/all-MiniLM-L6-v2 and nvidia/nv-embedqa-e5-v5).
Implement the candidate retrieval stage using these embedding models to retrieve the top-k relevant passages for a given query.
Stage 2 - Reranking:
Choose at least two ranking models (e.g., cross-encoder/ms-marco-MiniLM-L-12-v2 and nvidia/nv-rerankqa-mistral-4b-v3).
Implement the reranking stage to reorder the retrieved passages based on relevance scores from the ranking models.

Benchmarking and Evaluation:
Evaluate the performance of the retrieval pipeline using metrics like NDCG@10.
Compare the retrieval accuracy with and without the ranking models.
Analyze the impact of different embedding and ranking model combinations on retrieval accuracy.
