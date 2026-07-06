# \# 🩺 Medical LLM Fine-Tuning with Qwen2.5-1.5B-Instruct using QLoRA on PubMedQA

# 

# A lightweight and memory-efficient pipeline for fine-tuning \*\*Qwen2.5-1.5B-Instruct\*\* on the \*\*PubMedQA\*\* biomedical question-answering dataset using \*\*4-bit QLoRA\*\*. This project is designed to run on a single \*\*NVIDIA T4 (16 GB)\*\* GPU in Kaggle while maintaining strong performance with minimal computational resources.

# 

# \---

# 

# \## 📌 Overview

# 

# This repository demonstrates parameter-efficient fine-tuning (PEFT) of a large language model for biomedical question answering. The model is trained using the PubMedQA dataset with QLoRA, enabling efficient adaptation while significantly reducing GPU memory usage.

# 

# \### Key Features

# 

# \- ✅ Qwen2.5-1.5B-Instruct as the base model

# \- ✅ 4-bit Quantization (BitsAndBytes)

# \- ✅ QLoRA fine-tuning

# \- ✅ LoRA adapters for parameter-efficient training

# \- ✅ PubMedQA dataset integration

# \- ✅ Kaggle GPU (T4 16GB) compatible

# \- ✅ Hugging Face Hub upload support

# \- ✅ Automatic evaluation with validation loss and perplexity

# 

# \---

# 

# \## 📂 Repository Structure

# 

# ```

# .

# ├── Medical\_LLM\_Fine\_Tuning\_PubMedQA\_Qwen\_QLoRA.ipynb

# ├── medical-llm-fine-tuning-pubmedqa-qwen-qlora1.ipynb

# ├── README.md

# ├── LICENSE

# ├── .gitignore

# └── medical\_qwen/

# &#x20;   ├── adapter\_config.json

# &#x20;   ├── adapter\_model.safetensors

# &#x20;   ├── tokenizer.json

# &#x20;   ├── tokenizer\_config.json

# &#x20;   └── ...

# ```

# 

# \---

# 

# \## 🧠 Model Information

# 

# | Item | Value |

# |------|-------|

# | Base Model | Qwen2.5-1.5B-Instruct |

# | Fine-tuning | QLoRA |

# | Quantization | 4-bit |

# | Framework | Transformers + PEFT + TRL |

# | Task | Biomedical Question Answering |

# | Dataset | PubMedQA |

# | Platform | Kaggle |

# | GPU | NVIDIA Tesla T4 (16 GB) |

# 

# \---

# 

# \## 📊 Dataset

# 

# This project uses the \*\*PubMedQA\*\* dataset.

# 

# Training:

# \- `pqa\_artificial`

# 

# Evaluation:

# \- `pqa\_labeled`

# 

# The dataset consists of biomedical research questions paired with abstracts and corresponding answers.

# 

# \---

# 

# \## ⚙️ Training Configuration

# 

# | Parameter | Value |

# |-----------|-------|

# | Quantization | 4-bit |

# | LoRA | Enabled |

# | Gradient Checkpointing | Yes |

# | Optimizer | Paged AdamW 8-bit |

# | Max Sequence Length | 512 |

# | Mixed Precision | BF16 |

# | Device | GPU |

# 

# \---

# 

# \## 🛠️ Tech Stack

# 

# \- Python

# \- PyTorch

# \- Hugging Face Transformers

# \- PEFT

# \- TRL

# \- Accelerate

# \- BitsAndBytes

# \- Datasets

# \- Evaluate

# 

# \---

# 

# \## 🚀 Running the Notebook

# 

# \### 1. Clone the repository

# 

# ```bash

# git clone https://github.com/jakirniloy/medical\_qwen.git

# cd medical\_qwen

# ```

# 

# \### 2. Open the notebook

# 

# Run either notebook in:

# 

# \- Kaggle

# \- Google Colab

# \- Local Jupyter Notebook

# 

# \### 3. Enable GPU

# 

# For Kaggle:

# 

# \- Accelerator → GPU T4 x1

# \- Internet → ON

# 

# \### 4. Install dependencies

# 

# ```bash

# pip install transformers datasets peft trl accelerate bitsandbytes evaluate

# ```

# 

# \---

# 

# \## 📈 Evaluation

# 

# The notebook reports:

# 

# \- Training Loss

# \- Validation Loss

# \- Perplexity

# \- Mean Token Accuracy

# 

# Example:

# 

# | Metric | Value |

# |--------|------:|

# | Training Loss | 3.30 |

# | Validation Loss | 3.49 |

# | Perplexity | 32.90 |

# | Mean Token Accuracy | 59.3% |

# 

# \---

# 

# \## 💾 Saving the Model

# 

# The trained LoRA adapter is saved locally as

# 

# ```

# /kaggle/working/medical\_qwen

# ```

# 

# and can be uploaded directly to the Hugging Face Hub.

# 

# \---

# 

# \## 🤗 Hugging Face Upload

# 

# The notebook includes an optional section for pushing the trained adapter to Hugging Face.

# 

# Simply configure:

# 

# ```python

# HF\_USERNAME = "your\_username"

# HF\_TOKEN = "your\_huggingface\_token"

# ```

# 

# and execute the upload cell.

# 

# \---

# 

# \## 📌 Future Improvements

# 

# \- Full model merging

# \- RAG integration

# \- Medical benchmark evaluation

# \- Multi-turn clinical dialogue

# \- Quantitative comparison with other LLMs

# \- Deployment using Gradio or Streamlit

# 

# \---

# 

# \## 📄 License

# 

# This project is released under the \*\*GPL-3.0 License\*\*.

# 

# \---

# 

# \## 🙋 Author

# 

# \*\*Md. Jakir Hossain\*\*

# 

# GitHub: https://github.com/jakirniloy

# 

# \---

# 

# \## ⭐ Citation

# 

# If you find this repository useful for your research, please consider giving it a ⭐ on GitHub.

# 

# ```

# 

# \### I also recommend changing your repository name from:

# 

# ```

# medical\_qwen

# ```

# 

# to something more professional, such as:

# 

# \- \*\*Medical-LLM-Fine-Tuning-Qwen-QLoRA\*\*

# \- \*\*Qwen-PubMedQA-QLoRA\*\*

# \- \*\*Medical-Qwen-QLoRA\*\*

# \- \*\*Biomedical-LLM-Qwen\*\*

# \- \*\*MedicalLLM-PubMedQA\*\*

# 

# These names are more descriptive and improve discoverability for recruiters and researchers.

