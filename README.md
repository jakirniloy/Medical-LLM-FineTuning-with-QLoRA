# \# 🩺 Medical LLM Fine-Tuning with Qwen2.5-1.5B-Instruct using QLoRA

# 

# > Parameter-efficient fine-tuning of \*\*Qwen2.5-1.5B-Instruct\*\* on the \*\*PubMedQA\*\* biomedical question answering dataset using \*\*4-bit QLoRA\*\*.

# 

# \---

# 

# \## 🚀 Features

# 

# \- ✅ Qwen2.5-1.5B-Instruct

# \- ✅ QLoRA Fine-Tuning

# \- ✅ 4-bit Quantization (BitsAndBytes)

# \- ✅ PEFT (LoRA)

# \- ✅ PubMedQA Dataset

# \- ✅ Kaggle T4 GPU Compatible

# \- ✅ Hugging Face Integration

# \- ✅ Medical Question Answering

# 

# \---

# 

# \## 📂 Repository Structure

# 

# ```text

# .

# ├── Medical\_LLM\_Fine\_Tuning\_PubMedQA\_Qwen\_QLoRA.ipynb

# ├── medical-llm-fine-tuning-pubmedqa-qwen-qlora1.ipynb

# ├── medical\_qwen/

# ├── README.md

# ├── LICENSE

# └── .gitignore

# ```

# 

# \---

# 

# \## 🧠 Model

# 

# | Item | Value |

# |------|-------|

# | Base Model | Qwen2.5-1.5B-Instruct |

# | Task | Biomedical Question Answering |

# | Dataset | PubMedQA |

# | Fine-tuning | QLoRA |

# | Quantization | 4-bit |

# | Framework | Transformers + PEFT |

# | Platform | Kaggle |

# 

# \---

# 

# \## 📊 Dataset

# 

# \- \*\*Training:\*\* `pqa\_artificial`

# \- \*\*Evaluation:\*\* `pqa\_labeled`

# 

# The model is trained to answer biomedical questions using scientific abstracts from PubMed.

# 

# \---

# 

# \## ⚙️ Installation

# 

# ```bash

# git clone https://github.com/jakirniloy/medical\_qwen.git

# cd medical\_qwen

# 

# pip install transformers datasets peft trl accelerate bitsandbytes evaluate

# ```

# 

# \---

# 

# \## ▶️ Run

# 

# Open the notebook in:

# 

# \- Kaggle

# \- Google Colab

# \- Jupyter Notebook

# 

# Enable GPU before training.

# 

# \---

# 

# \## 📈 Example Training Results

# 

# | Metric | Value |

# |--------|-------|

# | Training Loss | 3.30 |

# | Validation Loss | 3.49 |

# | Validation Perplexity | 32.90 |

# | Mean Token Accuracy | 59.3% |

# 

# \---

# 

# \## 💾 Output

# 

# The trained adapter is saved as:

# 

# ```text

# /kaggle/working/medical\_qwen

# ```

# 

# \---

# 

# \## 🤗 Upload to Hugging Face

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

# \## 🛠 Tech Stack

# 

# \- Python

# \- PyTorch

# \- Hugging Face Transformers

# \- PEFT

# \- TRL

# \- Accelerate

# \- BitsAndBytes

# \- Datasets

# 

# \---

# 

# \## 📄 License

# 

# GPL-3.0 License

# 

# \---

# 

# \## 👨‍💻 Author

# 

# \*\*Md. Jakir Hossain\*\*

# 

# GitHub: https://github.com/jakirniloy

# 

# \---

# 

# ⭐ If you find this project useful, please consider giving it a star!

