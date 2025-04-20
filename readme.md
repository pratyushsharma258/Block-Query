# Block-Query: Advanced Blockchain Question-Answering System

[![NLP](https://img.shields.io/badge/NLP-Question%20Answering-blue)]()
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0+-green)]()
[![Transformers](https://img.shields.io/badge/🤗%20Transformers-Latest-yellow)]()

## 🔍 Overview

Block-Query is a specialized question-answering system focused on blockchain technologies. This project leverages state-of-the-art natural language processing models to provide accurate and comprehensive answers to blockchain-related queries, with particular emphasis on Ethereum private networks, Web3 development, and distributed application architectures. With an initial development using traditional LSTM architecture as well.

## 🧠 Models

The project includes implementations and fine-tuning of several advanced language models:

- **BART**: Facebook's Bidirectional Auto-Regressive Transformer for sequence-to-sequence tasks
- **T5**: Google's Text-to-Text Transfer Transformer
- **Flan-T5**: Google's instruction-tuned version of the T5 model
- **Pegasus**: State-of-the-art model for abstractive summarization
- **LSTM**: Recurrent neural network architecture for sequential data processing

Each model is implemented in its own Jupyter notebook ([BART.ipynb](BART.ipynb), [T5.ipynb](T5.ipynb), [Flan-T5.ipynb](Flan-T5.ipynb), [Pegasus.ipynb](Pegasus.ipynb), [LSTM.ipynb](LSTM.ipynb)) with detailed training, evaluation, and inference pipelines.

## 📊 Dataset

The system is trained on a comprehensive blockchain dataset containing AI generated Q&A pairs covering:

- Ethereum network setup and management
- Smart contract development
- Truffle framework usage
- Web3.js implementation
- IPFS integration
- Corda development
- And many other blockchain development topics sourced from the book Mastering BlockChain by Imran Bashir(2nd Edition)

Data is organized by chapters in JSON format in the [dataset](dataset) directory, with an augmented version available as [df_augmented.csv](dataset/df_augmented.csv).

## 🛠️ Setup and Requirements

Each model has its own requirements file:

- [requirements_BART.txt](requirements_BART.txt)
- [requirements_T5.txt](requirements_T5.txt)
- [requirements_Pegasus.txt](requirements_Pegasus.txt)
- [requirements_LSTM.txt](requirements_LSTM.txt)

To set up the environment for a specific model:

```bash
pip install -r requirements_<MODEL>.txt
```

## 🚀 Usage

1. **Environment Setup**: Install the requirements for your chosen model
2. **Model Training**: Open the corresponding notebook and run the training cells
3. **Inference**: Use the trained models to generate answers for blockchain queries
4. **Evaluation**: Assess model performance using integrated BLEU, ROGUE and other metrics

## 🏆 Model Performance

The implemented models have been trained on blockchain-specific data with the following hyperparameters:

- Max source length: 50
- Max target length: 200
- Learning rate: 1e-4

Performance is evaluated using various scores to measure the quality of generated answers against expert-provided references.

## 🤝 Contributing

Contributions to enhance the model performance, expand the dataset, or improve documentation are welcome. Please feel free to submit a pull request or open an issue.
