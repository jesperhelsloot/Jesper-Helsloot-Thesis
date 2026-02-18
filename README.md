Jesper Helsloot Thesis Code
Introduction

This repository contains the thesis code developed by Jesper Helsloot. The purpose of this project is to provide a structured and reproducible implementation of the experiments, workflows, and analyses conducted during the thesis research.

This codebase is intended for future thesis students who will extend, modify, or build upon this work. The goal of this README is to help you quickly understand the structure, dependencies, and workflow so you can efficiently continue development.

Table of Contents

Project Overview

Repository Structure

Installation

Usage

Workflow Description

Dependencies

Configuration

Extending the Project

Troubleshooting

Contributors

Project Overview

This repository primarily consists of:

A Jupyter Notebook (workflow.ipynb) containing:

Data processing steps

Model implementation and/or analysis

Experimental pipeline

Result evaluation and visualization

The notebook serves as the central workflow for reproducing the thesis results.

Repository Structure
.
├── workflow.ipynb     # Main thesis workflow notebook
└── README.md          # Project documentation


If additional datasets, scripts, or models are added later, they should follow a clear structure such as:

data/
src/
models/
results/


Future contributors are encouraged to keep the structure clean and modular.

Installation
1. Clone the Repository
git clone <repository-url>
cd <repository-folder>

2. Create a Virtual Environment (Recommended)
python -m venv venv


Activate it:

Windows:

venv\Scripts\activate


macOS/Linux:

source venv/bin/activate

3. Install Dependencies

If a requirements.txt file exists:

pip install -r requirements.txt


Otherwise, install required packages manually based on the notebook imports.

Usage
Running the Notebook

Open the project in Visual Studio Code.

Ensure the correct Python interpreter is selected.

Open workflow.ipynb.

Run cells sequentially from top to bottom.

Alternatively, use Jupyter:

jupyter notebook


Then open workflow.ipynb.

Workflow Description

The notebook follows a typical research pipeline:

Data loading

Data preprocessing

Feature engineering (if applicable)

Model implementation / algorithm execution

Evaluation

Visualization of results

It is recommended to:

Run cells sequentially.

Avoid executing cells out of order unless you fully understand the dependencies.

Refactor reusable code into separate Python modules if the project grows.

Dependencies

Dependencies are determined by the imports in workflow.ipynb. Common libraries in thesis projects typically include:

numpy

pandas

matplotlib

scikit-learn

torch or tensorflow (if deep learning is used)

To extract exact dependencies, inspect the first import cells of the notebook and generate a requirements.txt file:

pip freeze > requirements.txt


Future students are encouraged to maintain a pinned requirements.txt for reproducibility.

Configuration

If the notebook relies on:

File paths

Dataset locations

Model checkpoints

External APIs

These should be centralized at the top of the notebook in a dedicated configuration section.

For future improvements, consider:

Moving configuration to a .yaml or .json file.

Using environment variables for sensitive or system-specific paths.

Extending the Project

If you are continuing this thesis work:

Do not overwrite original experimental results.

Create new notebooks for major experimental branches.

Version control large changes.

Document any methodological changes clearly.

Recommended improvements for future students:

Modularize repeated code into /src.

Add automated evaluation scripts.

Add experiment logging (e.g., MLflow, Weights & Biases).

Add reproducibility notes.

Troubleshooting
Kernel Issues

Ensure the correct Python interpreter is selected.

Restart the kernel and run all cells again.

Dependency Conflicts

Recreate the virtual environment.

Pin exact versions in requirements.txt.

File Path Errors

Use relative paths instead of absolute paths.

Ensure datasets are placed in the expected directory.

Contributors

Jesper Helsloot (Thesis Author)

Future contributors should add themselves here when extending the project.

License

No license has been specified for this repository.

Usage and continuation are intended for academic thesis development.
