# Efficient Domain-Specific Fine-Tuning of Small Language Models 

## ✨ Overview

This repository supports the research paper:  
**"Parameter-Efficient Fine-Tuning of Small Language Models for Financial Risk Management: A Study on AML/KYC and Sanctions Screening Tasks"**.  

It includes code, datasets, and experiments for fine-tuning small language models (1-7B parameters) using:
- QLoRA
- LoRA 
- AdaLoRA  

for financial risk management tasks.

## 🚀 Key Features

- **Dataset**: 9,000 synthetic instruction-response pairs for:
  - AML
  - KYC 
  - Sanctions screening
  - Regulatory reasoning
  
- **Models**:
  - SmolLM3-3B
  - Llama-3.2-1B
  - Qwen2.5-1.5B

- **PEFT Methods**:
  - QLoRA
  - LoRA
  - AdaLoRA (with optimized configurations)

- **Evaluation**:
  - Standard metrics (BLEU, ROUGE, F1)
  - Domain-specific metrics (e.g., ROC-AUC for sanctions)

- **Reproducibility**: Runs on free-tier Google Colab (T4 GPU)

## 🛠️ Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/efficient-domain-tuning
cd efficient-domain-tuning

# Install dependencies
pip install -r requirements.txt

# Generate dataset
python src/data/domain_datasets.py

# Run QLoRA experiment
bash experiments/financial/run_qlora.sh
```

## 📂 Repository Structure

```
src/                 # Core code for data processing, training, and evaluation
experiments/         # Scripts and results for financial, legal, and medical domains
data/                # Synthetic datasets and processed instruction files
notebooks/           # Jupyter notebooks for analysis and visualization
docs/                # Detailed guides for installation, experiments, and contributions
```

## 📝 Citation

```bibtex
@article{souptikchakraborty,
  title={Parameter-Efficient Fine-Tuning of Small Language Models for Financial Risk Management},
  author={Souptik Chakraborty},
  journal={arXiv preprint arXiv:2025.xxxxx},
  year={2025}
}
```

## 🤝 Contributing

See [docs/contribution_guide.md](docs/contribution_guide.md) for guidelines. We welcome contributions in:
- Dataset creation
- Evaluation metrics
- Model optimizations

## 📧 Contact

For collaboration inquiries: [souptikc80@gmail.com](mailto:souptikc80@gmail.com)

---

### 📜 Installation Guide

See detailed installation instructions in [docs/installation.md](docs/installation.md)

**Requirements**:
- Python 3.8+
- NVIDIA GPU (T4 or better) with CUDA 11.7+
- Google Colab (free-tier) or local setup with 15GB VRAM / Kaggle Free Tier of 30 Hours per week
```
