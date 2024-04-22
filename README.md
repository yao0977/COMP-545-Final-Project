# COMP 545 & LING 782 Final Project

This repository contains the code for analyzing the representation biases in language models, focusing on the semantic similarity of country names based on frequency, GDP, and embeddings generated from various models such as BERT, DistilBERT, GPT-2, and T5.

## Getting Started

### Prerequisites

The code is written in Python and requires packages like `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, and `torch`. You can install all required packages using:

```bash
pip install numpy matplotlib seaborn scikit-learn torch
```

### Installation

Clone this repository to your local machine using:

```bash
git clone https://github.com/yao0977/COMP-545-Final-Project.git
```

Navigate into the project directory:

```bash
cd your-repository-name
```

### Setting up the Environment

In order to run the code, you need to create a directory `/content/drive/MyDrive/Colab Notebooks/country_distortions/Section_3_4` in your Google Drive and put the following files into it:

- `bert_test.csv`
- `distillbert_test.csv`
- `filtered_country_sentences.csv`
- `gpt2_test.csv`
- `t5_test.csv`

You also need to create a directory `/content/drive/MyDrive/Colab Notebooks/country_distortions/Section_5/model_prediction_results` in your Google Drive and put the following files into it:

- `original_results_100.csv`
- `distillbert_results_100.csv`
- `gpt_results_100.csv`
- `t5_results_100.csv`
 
These files contain the necessary data for running the experiments and should be placed in the specified directory to ensure the scripts can locate and utilize them correctly.

## Documentation

Further details on the code structure and specific functions are provided within the code files through comprehensive commenting. This documentation is intended to make it easier for users to understand and replicate the experiments.

### Important Information for TAs

For grading and review purposes, please focus on the `COMP545_final_project.ipynb` file and `fill_mask_task_analysis.ipynb` file. 

For `COMP545_final_project.ipynb`, specific sections that require attention include:

- **LLM Initialization**: Overview of how language models are initialized for the project.
- **Embedding**: Details on how embeddings are generated from each model.
- **In-vocabulary**: Explanation and analysis of vocabulary coverage across different models.
- **Semantic Similarities**: Comprehensive analysis of semantic similarities between country names across models. The functions `analyze_gdp_vs_semantic_similarity_with_line` and `analyze_gdp_vs_semantic_similarity_with_p_value`, along with their subsequent results, are optional for review. We determined that the results from these analyses were not statistically significant, and thus they may be less relevant for understanding the core outcomes of the project.

For `fill_mask_task_analysis.ipynb`, specific sections that require attention include:

- **Initialize BERT and BERT-like**, **Initialize GPT2**, and **Initialize T5**: Overview of how language models are initialized for the project.
- **Make predictions**: A combination of inherent measure to calculate prediction score provided by the original authors and curtailed measures for GPT-2 and T5 models.
- **Richer Countries are More Frequently Predicted**: Calculation of the proporation of the least 10 and top 10 frequently mentioned countries in the whole dataset - relevant to main arguments of the project.
- **Figure 3**: Visualization of the relationship between the number of correct model prediction and logged GDPs of countries - relevant to the main arguments of the project.
- Other parts are optional for review since they are only responsible for reading file and checking outputs.

## Notes about Release

This project does not include a PyPi package as it is tailored for research purposes and relies on specific data structures and setups that are not universally applicable as a standalone library. 

## Acknowledgments

Thanks to all contributors who have provided insights and feedback on this project.
