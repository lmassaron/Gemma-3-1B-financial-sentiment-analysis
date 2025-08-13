# Gemma-1B-financial-sentiment-analysis

This repository contains the code and resources for the project "Fine-Tuning Gemma 3 1B-IT for Financial Sentiment Analysis," a step-by-step guide on how to fine-tune Google's Gemma 1B-IT model for financial sentiment analysis.

You can find a detailed description of the project by reading my Medium article:
* [Fine-Tuning Gemma 3 1B-IT for Financial Sentiment Analysis: A Step-by-Step Guide](https://medium.com/@lucamassaron/fine-tuning-gemma-3-1b-it-for-financial-sentiment-analysis-a-step-by-step-guide-1a025d2fc75d)

![Gemma in finance](./gemma.png)

## Featured by Google for Developers

This project was featured by Google for Developers. You can find the post [here](https://www.linkedin.com/posts/googledevelopers_struggling-to-gauge-market-sentiment-activity-7356800131146358786-THaL).

![Gemma in finance](./gemma.png)

## Introduction

Sentiment analysis in the financial domain is a critical task for businesses and investors. It provides valuable insights into market trends, investor confidence, and consumer behavior. This project demonstrates how to fine-tune the Gemma 1B-IT model, a lightweight and powerful language model from Google, to perform sentiment analysis on financial and economic information.

The project uses the FinancialPhraseBank dataset, a collection of about 5,000 sentences from financial news, annotated with sentiment labels (positive, negative, or neutral).

## The Power of Gemma

Gemma is a family of lightweight, state-of-the-art open AI models from Google. The 1B Instruct version of Gemma is designed for instruction-based tasks, making it an ideal choice for this project. Gemma's key features include:

*   **High Performance:** Gemma delivers high performance while being resource-efficient.
*   **Instruction-Tuned:** The model is specifically tuned to follow instructions, which is perfect for sentiment analysis.
*   **Accessible:** Gemma can run on consumer hardware with a single GPU, making it accessible to a wide range of developers.

## Methodology

The project follows a structured approach to fine-tuning the Gemma model:

1.  **Dataset Preparation:** The FinancialPhraseBank dataset is loaded and preprocessed to create training, validation, and test sets.
2.  **Baseline Evaluation:** The pre-trained Gemma model is evaluated on the test set to establish a baseline performance.
3.  **Fine-Tuning:** The model is fine-tuned using Parameter-Efficient Fine-Tuning (PEFT) and Low-Rank Adaptation (LoRA). These techniques allow for efficient fine-tuning of large language models with limited computational resources.
4.  **Evaluation:** The fine-tuned model is evaluated on the test set, and the results are compared to the baseline.

## Results

The fine-tuning process significantly improves the model's performance. The accuracy of the model on the test set increases from **55%** (baseline) to over **85%** after fine-tuning. This demonstrates the effectiveness of fine-tuning even smaller models like Gemma 1B-IT for specific tasks.

## How to Use

To use this project, follow these steps:

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/lucamassaron/Gemma-1B-financial-sentiment-analysis.git
    ```

2.  **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Jupyter Notebook:**

    ```bash
    jupyter notebook fine-tune-gemma-3-1b-it-for-sentiment-analysis.ipynb
    ```

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

*   The FinancialPhraseBank dataset was created by the Aalto University School of Business.
*   This project uses the Hugging Face Transformers, PEFT, and TRL libraries.
