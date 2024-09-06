# Fine-Tuning-LLMs-using-QLoRA
# Fine-Tuning LLMs with LoRA

This project demonstrates how to fine-tune large language models (LLMs) such as **LLaMA** and **BERT** using **LoRA (Low-Rank Adaptation)** with the **PEFT (Parameter-Efficient Fine-Tuning)** method. The models are fine-tuned on different tasks using Hugging Face's `transformers` library and PyTorch.

## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Training LLaMA Model](#training-llama-model)
- [Training BERT Model](#training-bert-model)
- [License](#license)

## Project Overview
In this project, we fine-tune two different models:
- **LLaMA** for causal language modeling using the **wikitext** dataset.
- **BERT** for sequence classification using the **IMDB movie reviews** dataset.

We leverage **LoRA**, a technique that allows efficient fine-tuning by reducing the number of trainable parameters, making the process more computationally efficient.

## Technologies Used
- Python
- Hugging Face `transformers`
- `datasets`
- `PEFT (Parameter-Efficient Fine-Tuning)`
- PyTorch
- `accelerate`

## Installation

To set up this project, you need to install the required dependencies listed in the `requirements.txt` file.

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/llm-fine-tuning-lora.git
    cd llm-fine-tuning-lora
    ```

2. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Make sure to have access to a GPU for efficient fine-tuning.
2. Run the notebook to fine-tune either **LLaMA** or **BERT** models.
   
To train **LLaMA** and **BERT**, you can directly run the code in the notebook or use a Python script based on the notebook's content.

## Training LLaMA Model

To fine-tune the LLaMA model using the **Wikitext** dataset, load the LLaMA model, configure LoRA, and start training. The training process involves:
- Loading the tokenizer and model.
- Applying LoRA configuration.
- Fine-tuning the model with reduced parameters for efficiency.

## Training BERT Model

For **BERT**, the sequence classification task is conducted using the **IMDB** dataset. The process is similar:
- Loading the tokenizer and model.
- Applying LoRA configuration for parameter-efficient tuning.
- Fine-tuning the model for binary classification.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
