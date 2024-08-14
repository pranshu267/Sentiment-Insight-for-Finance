# Sentiment-Insight-for-Finance

## Project Overview

**Sentiment Insight for Finance** is a project focused on classifying financial statements as positive or negative using advanced Large Language Models (LLMs). The project leverages LLaMA 3 8b and Mistral v3 7b models, fine-tuned specifically for financial sentiment analysis. By utilizing LoRA (Low-Rank Adaptation) and 4-bit quantization techniques, I achieved efficient fine-tuning while maintaining high performance.

## Features

- **Efficient Fine-Tuning**: Implements LoRA (Low-Rank Adaptation) and 4-bit quantization to reduce computational costs while preserving model accuracy.
- **Financial Domain Focused**: Tailored specifically for analyzing sentiment in financial statements.

### Fine-Tuning Approach

To fine-tune these models effectively using Unsloth library for sentiment classification, I employed:

- **LoRA (Low-Rank Adaptation)**: This technique allows us to adapt pre-trained models to our specific task with a minimal number of additional parameters.
- **4-bit Quantization**: Reduces the memory footprint of the models, enabling more efficient computation and deployment without a significant loss in accuracy.

## Data

The project uses FiQA and Financial PhraseBank datasets of financial statements, categorized into positive, neutral and negative sentiment. The data includes annual reports, earnings releases, and other relevant financial statments made by institutions.


## Results

Below is the comparison of accuracy before and after fine-tuning the models:

| Model   | Accuracy Before Fine-Tuning | Accuracy After Fine-Tuning |
|---------|-----------------------------|----------------------------|
| LLaMA   | 31.9%                        | 80.6%                      |
| Mistral | 53.6%                        | 84.3%                      |

From the results, we can observe that Mistral shows a higher improvement and better performance compared to LLaMA, making it more suited for this particular financial sentiment classification task.

These results demonstrate the effectiveness of using LoRA and 4-bit quantization for sentiment analysis in financial statements.

## To DO

Finetune Gemma 2 9b and compare the performance with these models.