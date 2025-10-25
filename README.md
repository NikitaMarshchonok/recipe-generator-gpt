#  Recipe Generator GPT

This project is a **recipe generation model** built using a fine-tuned version of `distilgpt2` from Hugging Face Transformers. It takes a short input prompt and generates cooking recipes in natural language.

##  Built With
- `distilgpt2` model from HuggingFace Transformers
- `pandas`, `datasets`, `transformers`, `gradio`
- Trained **locally on CPU** using MacBook Pro
- Used **~100,000 rows** extracted from the original RecipeNLG dataset (2.5GB) and preprocessed locally


##  Dataset

- Based on the [RecipeNLG dataset](https://recipenlg.cs.put.poznan.pl/)
- For training, a **smaller subset (100,000 recipes)** was created from the full dataset for efficiency
- Data was preprocessed and cleaned to retain only the ingredients list

##  Training Details

- Fine-tuned locally using Hugging Face `Trainer`
- Used `TrainingArguments` with 3 epochs, batch size = 8, `distilgpt2` as the base
- Training completed on **MacBook Pro with M2 Pro chip (CPU only)**
- **Future training will be performed on GPU** to increase generation quality and performance

##  Roadmap

-  Initial fine-tuning on CPU (done)
-  Migrate training to **GPU (Colab / cloud)** for better results
-  Add support for **image generation** via DALL·E / Stable Diffusion
-  Deploy demo via **Gradio** or Hugging Face Spaces
-  Add multi-language recipe generation (e.g., 🇷🇺 Russian, 🇮🇱 Hebrew)

##  Demo (WIP)

Will be available soon via a [Gradio](https://www.gradio.app/) demo interface.

## Author

Nikita M.
Telegram: @nikitamarshchonok
LinkedIn: https://www.linkedin.com/in/nikita-marshchonok


