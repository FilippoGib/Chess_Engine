# Deep Learning Chess Engine

![Project Status](https://img.shields.io/badge/status-work%20in%20progress-yellow.svg)
![Language](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Environment](https://img.shields.io/badge/Google_Colab-F9AB00?logo=googlecolab)

This repository documents the development of a chess engine built from the ground up using various deep learning architectures. This is an ongoing project that explores the evolution of model complexity for game AI, starting from a simple MLP and progressing towards state-of-the-art transformer models.

## Project Goal

The primary goal is to learn, implement, and benchmark different deep learning architectures for the complex task of chess position evaluation. By building each model, we can compare their performance, training requirements, and understanding of the game.
The final goal is, make the various model play each other using a simple minmax or alpha beta pruning 

---

## Project Roadmap

This project is being developed in stages. Each stage represents a different model architecture with increasing complexity.

### 1. Multi-Layer Perceptron (MLP)
* **Status:** **Complete**
* **File:** `Chess_Engine_MLP.ipynb`
* **Description:** A baseline model that takes a flattened board representation as input. This simple, fully-connected network serves as a "hello world" for chess AI and establishes a performance baseline.

### 2. Convolutional Neural Network (CNN)
* **Status:** **In Progress**
* **Description:** This model will treat the chessboard as an 8x8 image with multiple channels, one per piece type, one-hot encoded in the piece position. CNNs are naturally suited for recognizing spatial patterns, such as pawn structures, king safety, and piece formations.

### 3. Transformer
* **Status:** **Planned**
* **Description:** The final planned stage involves implementing a transformer-based model. By using attention mechanisms, this model can hopefully learn more complex and long-range relationships between pieces on the board. Also "if you can apply a transformer to it you should"

### 4. Future Ideas
* Experiment with SOTA solutions such as PPO, Deep-Q, etc.
* Hybrid architectures (e.g., CNN + Transformer)

---

## 🛠️ Technology Stack

* **Language:** Python 3
* **Core Libraries:**
    * `TensorFlow` / `Keras`
    * `python-chess` (for board representation, move generation, and PGN parsing)
    * `NumPy` (for data manipulation)
* **Environment:** Google Colab & Jupyter Notebooks

---

## 🚀 Getting Started

Since the project is developed in Google Colab notebooks, getting started is simple.

1.  **Clone the repository (optional):**
    ```bash
    git clone git@github.com:FilippoGib/Chess_Engine.git
    ```

2.  **Run in Google Colab:**
    * Navigate to [https://colab.research.google.com/](https://colab.research.google.com/).
    * Go to `File` > `Upload notebook...`.
    * Select the `.ipynb` file you wish to run (e.g., `Chess_Engine_MLP.ipynb`).
    * The notebook will install its own dependencies (like `python-chess`) using `!pip install` commands at the top.

3.  **Run Locally (Alternative):**
    If you prefer to run the notebook locally:
    ```bash
    # Install required libraries
    pip install jupyterlab tensorflow python-chess numpy

    # Launch Jupyter
    jupyter lab
    ```
    Then, open the notebook file from the Jupyter interface.

---

## Contributing

This is primarily a personal project for learning and experimentation. However, suggestions, feedback, and bug reports are always welcome!
