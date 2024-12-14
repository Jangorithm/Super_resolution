# Enhancing Vehicle License Plate Quality Using Super-Resolution

[![Python 3.8](https://img.shields.io/badge/python-3.8.10-blue.svg)](https://www.python.org/downloads/release/python-3810/)

License plate recognition from CCTV footage can vary in accuracy depending on the image quality. To address this issue, we introduce a method that utilizes Super-Resolution techniques to reconstruct low-quality license plate images into high-quality ones.


## 🚀 Features Included

- **[GitHub Actions](https://docs.github.com/en/actions)**: CI/CD workflows for testing code, deploying models, running experiments, and more.
- **Config Directory**: Centralized configuration files for the project.




---

## 📁 Detailed Directory Breakdown

- **`/config`**: Store all configuration files needed for your project.
  - Example: `config.yaml` can be used for setting up hyperparameters, API keys, or other environment variables.

- **`/data`**: Structured data folders for different stages of the project.
  - `raw/`: Raw data straight from the source.
  - `processed/`: Cleaned and preprocessed data ready for use in models.
  - `database/`: Database files if using local storage solutions.

- **`/iac`**: Infrastructure as Code scripts for automating cloud deployments (e.g., AWS CloudFormation, Terraform).

- **`/notebooks`**: Jupyter notebooks for performing Exploratory Data Analysis (EDA), experimenting with models, and reporting.
  - Example: `00_example.ipynb` shows how a notebook looks in the project.

- **`/results`**: Store experiment results, logs, and models.

- **`/src`**: Main source code for your project.
  - `/constants/`: Store project-wide constants (e.g., file paths, API endpoints).
  - `/models/`: Machine learning models (e.g., neural networks, decisi`on trees) scripts, classes, and functions.
  - `/pipelines/`: Data and model pipelines.
  - `/utils/`: Utility functions and helpers (e.g., data loaders, preprocessing functions).

- **`/tests`**: Unit and integration tests.

---

## ⚙️ Configuration Files

- **`.env`**: Store environment variables like API keys, database credentials, and sensitive information.

- **`.gitignore`**: Standard [`.gitignore`](https://git-scm.com/docs/gitignore) file to exclude unnecessary files (e.g., environment files, data files).

- **`.pre-commit-config.yaml`**: Configuration for [pre-commit](https://pre-commit.com/) hooks for linting, formatting, and type checking.

- **`docker-compose.yaml`**: A Docker Compose configuration to spin up services such as [MLflow](https://mlflow.org/), [Langfuse](https://www.langfuse.com/), databases, and any additional tools.

- **`pyproject.toml`**: Configuration of the project, plus the configuration for formatting and linting. This file is used by [uv](https://docs.astral.sh/uv/) to manage the project and [ruff](https://docs.astral.sh/ruff/) for linting and formatting.

- **`uv.lock`**: Lock file for [uv](https://docs.astral.sh/uv/) package manager automatically generated by `uv` when installing packages.

---

## 🛠️ How to Use

### 1. **Clone the Repository**
```bash
git clone https://github.com/username/ai-project-template.git
cd ai-project-template
```

### 2. **Install uv Package Manager**
- For macOS and Linux:
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```
- For Windows:
```bash
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

### 3. **Install Python**
```bash
uv install python
```

### 4. **Install Dependencies**
```bash
uv sync --all-extras --dev
```

### 5. Start Docker Compose Services (Optional)
```bash
docker-compose up -d
```


---

## 🗂️ Repository Structure
```bash
.
├── config                    # Configuration files for your project
│   └── config.yaml           # Example configuration file
├── data                      # Folder to store raw and processed data
│   ├── database              # Databases or local data storage
│   ├── processed             # Preprocessed/cleaned data
│   └── raw                   # Raw data inputs
├── iac                       # Infrastructure as Code (IaC) scripts for cloud deployment
├── notebooks                 # Jupyter notebooks for exploratory data analysis, experiments
│   └── 00_example.ipynb      # Example notebook
├── results                   # Folder to store the results of experiments and models
├── src                       # Source code of your project
│   ├── constants             # Constants used in the project
│   ├── models                # Machine learning model scripts
│   ├── pipelines             # ML pipelines for preprocessing and modeling
│   ├── utils                 # Utility functions
│   └── execution.py          # Main execution script
├── tests                     # Unit and integration tests
│   └── test_example.py       # Example test file using pytest
├── .env                      # Environment variables file
├── .gitignore                # Standard .gitignore file
├── .pre-commit-config.yaml   # Configuration for pre-commit hooks
├── docker-compose.yaml       # Docker Compose setup for MLflow, Langfuse, and related services
├── pyproject.toml            # Configuration for formatting, linting, type-checking, and testing
├── README.md                 # Documentation for the project (you're reading it!)
└── uv.lock                   # Lock file for uv package manager

```

---

## 📋 Contributing
Feel free to contribute to this project by submitting a pull request.
