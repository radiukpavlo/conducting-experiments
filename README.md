# Conducting Experiments in PyTorch

This repository is designed for conducting experiments, learning PyTorch fundamentals, and building modular machine learning workflows. It includes a comprehensive collection of Jupyter Notebooks, assignments, modular Python scripts, datasets, and resources for reproducible experiments.

## 🗂️ Project Structure

The project is organized into several distinct directories to guide you through different stages of learning and experimentation:

```
conducting-experiments-test/
├── 01_notebooks/                  # Core PyTorch tutorial notebooks (Fundamentals to Deployment)
├── 02_assignments/                # Exercise notebooks, prompts, and solutions
├── 03_archived/                   # Deprecated or old materials
├── going_modular/                 # Examples of converting Notebooks to modular Python scripts
├── tutorials/                     # Setup guides and helper functions
├── models/                        # Saved models and checkpoints
├── images/                        # Assets and diagrams
├── lecture-notes/                 # Additional theoretical materials
└── ...                            # Other configuration files (.gitignore, LICENSE, etc.)
```

## 🚀 Key Features

- **Hands-on Tutorials (`01_notebooks/`)**: Step-by-step Jupyter notebooks covering deep learning theory and PyTorch implementation, including Classification, Computer Vision, Custom Datasets, Paper Replicating, and Model Deployment.
- **Practical Assignments (`02_assignments/`)**: Test your understanding with structured exercises and verify your logic against provided solutions.
- **Modular Code (`going_modular/`)**: Learn how to transition from exploratory notebook environments to robust, production-ready Python scripts.
- **Reproducibility**: Emphasis on setting random seeds and organizing code for consistent experiment results across different environments.
- **Multilingual Setup (`tutorials/`)**: Contextual setup instructions provided in both English and Ukrainian, alongside standard helper functions.

## 🛠️ Getting Started

### Prerequisites

- Python 3.8+
- [PyTorch](https://pytorch.org/get-started/locally/)
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/radiukpavlo/conducting-experiments-test.git
   cd conducting-experiments-test
   ```

2. **Install dependencies:**
   Depending on your specific needs (and hardware limitations like CUDA availability), install the primary data science packages:

   ```bash
   pip install torch torchvision jupyter matplotlib pandas numpy scikit-learn
   ```

3. **Explore Notebooks:**

   ```bash
   jupyter notebook
   ```

## 📖 Usage

- Start by navigating to the `01_notebooks/` directory and opening `ce_01_pytorch_fundamentals.ipynb`. Follow the sequence of notebooks to gradually build your PyTorch skills.
- Once comfortable, reinforce your knowledge by attempting the assignments in `02_assignments/`.
- To learn ML engineering practices, look into `going_modular/` to see how code from the `01_notebooks/` directory translates to modular `.py` files.
- For guidance on environment setup, refer to:
  - `tutorials/SETUP_ENG.md` (English)
  - `tutorials/SETUP_UKR.md` (Ukrainian)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## 📄 License

This project is distributed under the MIT License. See the `LICENSE` file for more information.

---
*Happy experimenting with PyTorch!*
