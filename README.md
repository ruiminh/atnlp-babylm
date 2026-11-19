# atnlp-babylm
Group project for Advanced Topics in NLP: GPT-style language model training and evaluation.
We will implement and train a small GPT-style language model on the BabyLM Strict-Small dataset, evaluate its next-token prediction, and use the group implementation as the baseline for our individual research contributions.

## Project requirements

### Group baseline

As a group, we will:

1. Implement the Generative Pretrained Transformer architecture using the course boilerplate provided on Absalon.
2. Follow the boilerplate’s sanity checks to verify that the model is implemented correctly.
3. Load and tokenize the BabyLM Strict-Small data.
4. Build a data loader that batches examples efficiently and avoids wasted computation.
5. Train the model and evaluate next-token prediction using cross-entropy loss.
6. Compare our results with the expected course result.

The course slides give an expected validation loss of approximately **3.598 after one epoch**. We will follow the exact model, data, training, and validation protocol in the Absalon assignment materials when making this comparison.

### Group presentation

The group will record a **10-minute progress presentation** describing the project, implementation, experiments, and current results.

## Dataset

We use [BabyLM-community/BabyLM-2026-Strict-Small](https://huggingface.co/datasets/BabyLM-community/BabyLM-2026-Strict-Small) from Hugging Face.

The dataset is available through the Hugging Face `datasets` library. Downloaded data is cached by that library and should not be committed to this repository.

The course slide describes the dataset as “10M words,” while the Hugging Face dataset card describes it as 10 million tokens. We will check the Absalon assignment instructions for the exact dataset and counting convention required for our experiments.

## Evaluation

- **Intrinsic evaluation:** validation cross-entropy loss for next-token prediction.
- **Reference result:** approximately 3.598 validation loss after one epoch, as shown in the course slides. This is a comparison target; results depend on following the course’s specified setup.
- **Additional evaluation:** each student will design a new evaluation task for their individual research contribution. The course slides also introduce BLiMP as an example of linguistic acceptability evaluation; we will use it if required by the assignment or agreed by the group.

