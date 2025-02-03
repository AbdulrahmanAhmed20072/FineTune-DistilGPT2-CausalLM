# Fine-Tuning DistilGPT2 for Causal Language Modeling

This repository fine-tunes DistilGPT2 for causal language modeling using Parameter-Efficient Fine-Tuning (PEFT) with LoRA and BitsAndBytes quantization.

## Features

- **DistilGPT2 Fine-Tuning**: Adapts DistilGPT2 for text generation.
- **LoRA & BitsAndBytes**: Efficient training with low-rank adaptation and 4-bit quantization.
- **Dataset Preparation**: Uses the ELI5 dataset for training.
- **Training Pipeline**: Utilizes Hugging Face `Trainer` for efficient model training.
- **Evaluation**: Computes perplexity and accuracy metrics for model performance.

## Files

1. **`FineTune_DistilGPT2_LM.ipynb`**: Python script implementing the training pipeline.
2. **Dataset**: ELI5 dataset for text generation tasks.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdulrahmanAhmed20072/FineTune-DistilGPT2-CausalLM.git
   ```
2. Install the required dependencies:
   ```bash
   pip install datasets bitsandbytes accelerate evaluate transformers torch peft numpy
   ```

## Usage

1. Load and preprocess the dataset.
2. Fine-tune DistilGPT2 with LoRA and quantization.
3. Evaluate model performance.
4. Generate text using the trained model.

Run the script:
```bash
FineTune_DistilGPT2_LM.ipynb
```

## Outputs

- Fine-tuned DistilGPT2 model for text generation.
- Perplexity and accuracy evaluation on test data.
- Generated text samples for given prompts.

## Example

Prompt:
```
me and
```

Generated Text:
```
me and my friends went to the park and had a great time.
```
