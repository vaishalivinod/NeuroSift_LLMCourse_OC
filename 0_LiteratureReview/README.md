# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: [FLAN-T5 – Instruction-Finetuned Language Model]

  - **[Link](https://arxiv.org/pdf/2210.11416)**
  - **Objective**: To develop a general-purpose instruction-following model that performs well across a wide variety of tasks with minimal task-specific tuning.
  - **Methods**: FLAN-T5 was built by fine-tuning T5 on a curated mixture of instruction-based datasets, enabling it to generalize to unseen prompts.
  - **Outcomes**: The model showed strong performance on zero-shot and few-shot tasks like question answering and summarization.
  - **Relation to the Project**: NeuroSift uses FLAN-T5 to answer user-defined questions based on neuroscience PDF content, leveraging the model’s ability to generalize from instructions and context alone.

- **Source 2**: [Named Entity Recognition and Normalization Applied to Large-Scale Information Extraction from the Materials Science Literature]

  - **[Link](https://pubs.acs.org/doi/10.1021/acs.jcim.9b00470)**
  - **Objective**: To extract structured metadata (e.g., brain regions, methods, species) from domain-specific articles using NLP.
  - **Methods**:  The authors used custom pipelines combining Named Entity Recognition (NER), dictionary matching, and co-reference resolution across full-text articles.
  - **Outcomes**: Successfully created machine-readable material science metadata across thousands of articles, significantly aiding downstream search and retrieval.
  - **Relation to the Project**: This work, although done with Material Science literature, illustrates the demand and feasibility of extracting data from domain-specific articles. NeuroSift extends this with a question-answering paradigm using a general LLM for neuroscience litterature.

- **Source 3**: [SciFive: a text-to-text transformer model for biomedical literature]

  - **[Link](https://arxiv.org/abs/2106.03598)**
  - **Objective**: To adapt the T5 (Text-to-Text Transfer Transformer) architecture for biomedical NLP tasks by pretraining it on domain-specific corpora.
  - **Methods**: The SciFive model is trained on biomedical datasets to fine-tune the general-purpose T5 transformer. It is evaluated on various biomedical NLP tasks, including named entity recognition, relation extraction, natural language inference, and question answering.
  - **Outcomes**: SciFive achieves performance in multiple tasks, surpassing models like BERT, BioBERT, and base T5. It shows particular strength in tasks that involve complex or generative output, such as question answering.
  - **Relation to the Project**: This work demonstrates the effectiveness of domain-specific adaptation of text-to-text models, supporting NeuroSift’s approach of using generative models like Flan-T5 for biomedical question answering from scientific texts.
