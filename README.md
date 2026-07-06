# <div align="center">

# 

# \# 🩺 Medical LLM Fine-Tuning using Qwen2.5-1.5B \& QLoRA

# 

# \### Efficient Biomedical Question Answering using PubMedQA and Parameter-Efficient Fine-Tuning (PEFT)

# 

# <p align="center">

# 

# !\[Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge\&logo=python)

# !\[PyTorch](https://img.shields.io/badge/PyTorch-2.x-red?style=for-the-badge\&logo=pytorch)

# !\[Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow?style=for-the-badge\&logo=huggingface)

# !\[QLoRA](https://img.shields.io/badge/QLoRA-4bit-success?style=for-the-badge)

# !\[License](https://img.shields.io/badge/License-GPL--3.0-green?style=for-the-badge)

# 

# </p>

# 

# \---

# 

# ⭐ Fine-tuning \*\*Qwen2.5-1.5B-Instruct\*\* on \*\*PubMedQA\*\* using \*\*4-bit QLoRA\*\* for biomedical question answering.

# 

# </div>

# 

# \---

# 

# \# 📖 Overview

# 

# This project demonstrates how to efficiently fine-tune \*\*Qwen2.5-1.5B-Instruct\*\* for biomedical question answering using the \*\*PubMedQA\*\* dataset.

# 

# Instead of updating billions of parameters, this project uses \*\*QLoRA (Quantized Low-Rank Adaptation)\*\*, allowing training on a single \*\*NVIDIA Tesla T4 (16GB)\*\* GPU.

# 

# \---

# 

# \# ✨ Features

# 

# \- 🚀 Qwen2.5-1.5B-Instruct

# \- ⚡ 4-bit Quantization (BitsAndBytes)

# \- 🧠 QLoRA Fine-Tuning

# \- 🔥 LoRA Adapters

# \- 📚 PubMedQA Dataset

# \- 💻 Kaggle GPU Compatible

# \- 🤗 Hugging Face Integration

# \- 📊 Automatic Evaluation

# \- 📈 Validation Perplexity Calculation

# 

# \---

# 

# \# 🏗 Project Structure

# 

# ```text

# medical\_qwen/

# │

# ├── Medical\_LLM\_Fine\_Tuning\_PubMedQA\_Qwen\_QLoRA.ipynb

# ├── medical-llm-fine-tuning-pubmedqa-qwen-qlora1.ipynb

# ├── medical\_qwen/

# │   ├── adapter\_model.safetensors

# │   ├── adapter\_config.json

# │   ├── tokenizer.json

# │   ├── tokenizer\_config.json

# │   └── special\_tokens\_map.json

# │

# ├── README.md

# ├── LICENSE

# └── .gitignore

# ```

# 

# \---

# 

# \# 🧠 Model Information

# 

# | Property | Value |

# |-----------|-------|

# | Base Model | Qwen2.5-1.5B-Instruct |

# | Fine-tuning | QLoRA |

# | Quantization | 4-bit |

# | Framework | Transformers + PEFT |

# | Dataset | PubMedQA |

# | GPU | Tesla T4 (16GB) |

# | Language | English |

# | Task | Biomedical Question Answering |

# 

# \---

# 

# \# 📊 Dataset

# 

# | Split | Dataset |

# |--------|----------|

# | Training | pqa\_artificial |

# | Validation | pqa\_labeled |

# 

# The model learns to answer biomedical questions using scientific abstracts collected from PubMed.

# 

# \---

# 

# \# ⚙️ Training Pipeline

# 

# ```text

# PubMedQA

# &#x20;     │

# &#x20;     ▼

# Data Preprocessing

# &#x20;     │

# &#x20;     ▼

# Tokenization

# &#x20;     │

# &#x20;     ▼

# 4-bit Quantization

# &#x20;     │

# &#x20;     ▼

# QLoRA Fine-Tuning

# &#x20;     │

# &#x20;     ▼

# Model Evaluation

# &#x20;     │

# &#x20;     ▼

# Save LoRA Adapter

# ```

# 

# \---

# 

# \# 📈 Example Results

# 

# | Metric | Score |

# |---------|------:|

# | Training Loss | 3.30 |

# | Validation Loss | 3.49 |

# | Validation Perplexity | 32.90 |

# | Mean Token Accuracy | 59.3% |

# 

# \---

# 

# \# 🚀 Installation

# 

# ```bash

# git clone https://github.com/jakirniloy/medical\_qwen.git

# 

# cd medical\_qwen

# 

# pip install transformers datasets peft trl accelerate bitsandbytes evaluate

# ```

# 

# \---

# 

# \# ▶️ Run the Notebook

# 

# Open the notebook using:

# 

# \- Kaggle

# \- Google Colab

# \- Jupyter Notebook

# 

# Enable GPU before training.

# 

# \---

# 

# \# 💾 Output

# 

# After training, the adapter is saved to:

# 

# ```text

# /kaggle/working/medical\_qwen

# ```

# 

# \---

# 

# \# 🤗 Upload to Hugging Face

# 

# ```python

# from huggingface\_hub import upload\_folder

# 

# upload\_folder(

# &#x20;   folder\_path="/kaggle/working/medical\_qwen",

# &#x20;   repo\_id="YOUR\_USERNAME/medical\_qwen",

# &#x20;   repo\_type="model"

# )

# ```

# 

# \---

# 

# \# 🛠 Technology Stack

# 

# | Library | Purpose |

# |----------|---------|

# | PyTorch | Deep Learning |

# | Transformers | LLM |

# | PEFT | Parameter Efficient Fine-Tuning |

# | TRL | Supervised Fine-Tuning |

# | BitsAndBytes | 4-bit Quantization |

# | Accelerate | Multi-device Training |

# | Datasets | Dataset Loading |

# 

# \---

# 

# \# 📌 Future Work

# 

# \- \[ ] Merge LoRA with Base Model

# \- \[ ] RAG-based Medical QA

# \- \[ ] Streamlit Demo

# \- \[ ] Gradio Web App

# \- \[ ] Clinical Benchmark Evaluation

# \- \[ ] Multi-turn Medical Conversation

# 

# \---

# 

# \# 📄 License

# 

# This project is licensed under the \*\*GPL-3.0 License\*\*.

# 

# \---

# 

# \# 👨‍💻 Author

# 

# \*\*Md. Jakir Hossain\*\*

# 

# 🎓 AI Researcher | Medical AI | Large Language Models

# 

# GitHub: https://github.com/jakirniloy

# 

# \---

# 

# <div align="center">

# 

# \### ⭐ If you found this repository useful, please consider giving it a Star ⭐

# 

# </div>

