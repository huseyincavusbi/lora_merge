# lora_merge

A minimal notebook to merge a LoRA adapter into a base causal LM and push the merged model to the Hugging Face Hub.

## What this notebook does

- Loads a base causal LM and its tokenizer.
- Loads a LoRA adapter and merges it into the base model.
- Pushes the merged model and tokenizer to the Hugging Face Hub.

The notebook is set up to run in Colab.


## Requirements

- Python 3.8+ with GPU recommended for large models
- Packages: `transformers`, `peft`, `bitsandbytes`, `torch`, and `huggingface_hub` (install via `pip`).

## Notes and tips

- Replace the placeholder strings in the notebook before running.
- Keep your `HF_TOKEN` secret. Do not commit it into the repository.
- For very large models, prefer running in Colab Pro/Pro+ or a machine with sufficient GPU RAM.

## Quick Colab usage

If you want the fastest way to try this repository without installing packages locally, open the notebook in Colab and run the cells:

1. Click the Colab badge at the top of `lora_merge.ipynb` to open in Colab — use a GPU runtime (Runtime > Change runtime type > GPU). GPU is required.
2. Edit the placeholders (base model, adapter repo, merged repo) in the notebook cells.
3. Provide your Hugging Face token using Colab secrets.
4. Run the cells in order. Colab will install `bitsandbytes` and other required packages when needed.

Colab is recommended for quick experimentation, especially when you don't want to set up a local GPU environment.

## Authentication
Colab: the notebook uses Colab secrets  for the HF token by default.

## License

This project is licensed under the MIT License — see the `LICENSE` file.

