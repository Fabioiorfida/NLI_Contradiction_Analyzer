# Political Statement Analyzer (NLI & Explanatory Models)

A comprehensive toolkit for automatically assessing the logical consistency of political claims. The project leverages Natural Language Inference (NLI) to determine whether one statement contradicts, supports, or is neutral with respect to another, and employs a generative model to produce human‑readable explanations.

## Goals

* Identify the relationship (entailment, neutral, contradiction) between two political statements.
* Provide clear, natural‑language explanations supporting each classification.
* Store, retrieve, and analyse statements at scale through MongoDB integration.

## Key Features

* Fine‑tuned BERT model for fast, accurate NLI classification.
* Custom T5 model for automatic explanation generation.
* Modular Python interface designed for easy extension and testing.
* Bulk CSV import for swift dataset ingestion.
* Seamless MongoDB support for persistent storage and advanced querying.

## Requirements

* Python 3.8 or newer
* Packages: transformers, torch, pymongo, pandas
* MongoDB running on localhost (27017) or a custom URI
* Local copies of the fine‑tuned BERT and T5 models in the specified directories

## Project Structure

* OptimizedPoliticalStatementAnalyzer– core class managing models and database
* main.py – entry point for quick analysis
* BERT\_NLI\_Model – fine‑tuned BERT weights
* BERT\_NLI\_Tokenizer – corresponding tokenizer files
* T5\_Explanation\_Final – fine‑tuned T5 weights
* T5\_Explanation\_Tokenizer\_Final – corresponding tokenizer files
* political\_statements\_sample.csv – sample dataset
* README.md – this document

## How It Works

1. Configure model paths and database settings in main.py.
2. The BERT module classifies each statement pair.
3. The T5 module generates an explanation for the predicted label.
4. Results and metrics are showed.

## Typical Use Cases

* Monitoring shifts and inconsistencies in political discourse
* Supporting fact‑checking workflows in journalism
* Academic research on explainable AI and computational linguistics

## Contributing

Contributions are welcome! Feel free to open issues for questions or improvements and submit pull requests for bug fixes or new features.

## Author

Fabio Iorfida – MSc in Music Informatics & Computer Science

For enquiries, please use the Issues section of the repository.

## License

Distributed under the MIT License. See the LICENSE file for full details.
