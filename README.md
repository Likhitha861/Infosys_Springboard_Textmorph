# Infosys_Springboard_Textmorph
Milestone 1 – Text Summarization & Paraphrasing
Overview

This milestone is part of the Infosys TextMorph Advanced Text Summarization and Paraphrasing Program.
The goal is to implement, evaluate, and compare advanced NLP models for text summarization and text paraphrasing.

Approach

We experimented with three pretrained models for summarization and three for paraphrasing:

🔹 Text Summarization

T5 Base

BART Base

Pegasus-xsum

🔹 Text Paraphrasing

T5 Paraphrase

BART Paraphrase

Pegasus Paraphrase

Each model was loaded using the Hugging Face transformers library. Summarization tasks used prefixes like "summarize:" and paraphrasing tasks used "paraphrase:" where applicable.

🔎 Methodology

--Dataset Preparation:

Input text was taken from at least two .txt files.

The text passages were cleaned and stored for testing across all models.

--Model Implementation:

Loaded T5, BART, and Pegasus models along with their tokenizers.

Defined helper functions for summarization and paraphrasing.

Used beam search for improved output quality.

--Evaluation & Comparison:

Ran each model on the same input files.

Collected summaries and paraphrases for comparison.

--Generated plots to compare:

Summary length distribution

Inference time per model

Basic similarity metrics (e.g., ROUGE or cosine similarity)

--Visualization:

Plots were created to highlight differences in performance.

Comparison tables were included to show variation in summaries and paraphrases.

📊 Observations

--Summarization:

T5 Base: Balanced outputs, fluent, but sometimes generic.

BART Base: Produced detailed summaries, slightly longer than T5.

Pegasus-xsum: Generated very concise and abstractive summaries, often closer to human-style writing.

--Paraphrasing:

T5 Paraphrase: Good rewording, but often close to the original structure.

BART Paraphrase: Produced more diverse rephrasings with natural fluency.

Pegasus Paraphrase: Best variation across outputs, strong in generating novel sentence structures.

--General Findings:

Pegasus models are more abstractive and creative, while T5 and BART balance fluency and faithfulness.

Beam search improves quality but increases computation time.

Visualizations clearly show trade-offs between models in terms of length, diversity, and runtime.
