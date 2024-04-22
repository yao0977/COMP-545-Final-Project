# COMP 545 & LING 782 Final Project

# Semantic Similarity Analysis in Language Models

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

These files contain the necessary data for running the experiments and should be placed in the specified directory to ensure the scripts can locate and utilize them correctly.

## Usage

To run the semantic similarity analysis, execute the Python scripts provided in the repository. Each script corresponds to different parts of the analysis for each model:

```bash
python run_analysis.py
```

This command will initiate the processing and analysis based on the pre-defined configurations in the script.

## Documentation

Further details on the code structure and specific functions are provided within the code files through comprehensive commenting. This documentation is intended to make it easier for users to understand and replicate the experiments.

### Important Information for TAs

For grading and review purposes, please focus on the `COMP545_final_project.ipynb` file and `fill_mask_task_analysis.ipynb` file. For `COMP545_final_project.ipynb`, specific sections that require attention include:

- **LLM Initialization**: Overview of how language models are initialized for the project.
- **Embedding**: Details on how embeddings are generated from each model.
- **In-vocabulary**: Explanation and analysis of vocabulary coverage across different models.
- **Semantic Similarities**: Comprehensive analysis of semantic similarities between country names across models. The functions `analyze_gdp_vs_semantic_similarity_with_line` and `analyze_gdp_vs_semantic_similarity_with_p_value`, along with their subsequent results, are optional for review. We determined that the results from these analyses were not statistically significant, and thus they may be less relevant for understanding the core outcomes of the project.

## Notes about Release

This project does not include a PyPi package as it is tailored for research purposes and relies on specific data structures and setups that are not universally applicable as a standalone library. 

## Acknowledgments

Thanks to all contributors who have provided insights and feedback on this project.


-----------------------------------









You will release your code on GitHub, and make it public only at the end of your project. Do not copy and paste solutions from your assignment, but you may reuse what you learned and refine it beyond what was in the assignment. You must include all the instructions either in the readme, or in a separate file that is linked in the readme if it’s too long. Make sure to indicate what the TAs should be reading as you may have instructions beyond the scope of our grading. To have an idea of what you should include, please refer to this checklist: https://github.com/paperswithcode/releasing-research-code

● Release usable code\
● Avoid instructions that only work on specific platforms (e.g. SLURM)\
● Provide self-contained instructions that are straightforward to follow\
● Release code on GitHub (if it’s private, invite @xhluca or @ncmeade)\
● Include instructions in Readme, or link to separate markdown file with full instructions\
● Indicate what the TA should be reading\
● Wrote the code in Python\
● Released a PyPi package with instructions (if it’s not relevant, explain why in the GitHub readme, in a section called “Notes about release”)\
  ○ For others to run the experiments\
  ○ To import and reuse parts of the code as a standalone library\
  ○ Can be installed via `pip` from the official PyPi
