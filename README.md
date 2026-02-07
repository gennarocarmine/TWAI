# T.W.A.I. - Tris Was Already Invented

**T.W.A.I.** (Tris Was Already Invented) is an implementation of the classic **Connect 4** game that benchmarks two distinct Artificial Intelligence philosophies: the classical symbolic approach (**Minimax**) versus the modern data-driven approach (**MLP Neural Network**).

This project was developed for the **Foundations of Artificial Intelligence** course at the University of Salerno.

---

## 🚀 Installation

Follow these steps to run the application on your local machine.

### Prerequisites

Ensure you have [Python](https://www.python.org/) installed (version 3.8 or higher).

### 1. Clone the repository

```bash
git clone [https://github.com/gennarocarmine/fia-project.git](https://github.com/gennarocarmine/fia-project.git)
cd fia-project
```

### 2. Create a Virtual Environment (Recommended)

It is best practice to use a virtual environment to manage dependencies.

**Windows:**

```bash
python -m venv venv
.\venv\Scripts\activate
```

**Mac/Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

Install the required libraries (Streamlit, Scikit-learn, Pandas, etc.) using the provided file:

```bash
pip install -r requirements.txt
```

Or for Linux/Mac users:

```bash
pip3 install -r requirements.txt
```

### 4. Generate the Dataset ⚠️ (Crucial Step)

Before running the application, you must generate the training data. The Neural Network needs a dataset to learn from. Run the generation script which creates connect4_dataset_hq.csv via self-play simulations.

```bash
python generate_dataset.py
```

Or

```bash
python3 generate_dataset.py
```

> Note: This process might take a few moments as it simulates thousands of games to ensure high-quality data.

---

### 🎮 How to Run

Once the dataset is ready, you can launch the game interface. Ensure you are where `app.py` is located and run:

```bash
streamlit run app.py
```

Troubleshooting: If the command is not found or doesn't run, try using the module flag:

```bash
python -m streamlit run app.py
# Or: python3 -m streamlit run app.py
```

A browser tab will automatically open (usually at http://localhost:8501).

    Select Opponent: Choose between Minimax (Symbolic AI) or Neural Network (Machine Learning) from the sidebar.

    Play: Click the arrows above the grid to drop your pieces.

    Reset: Use the sidebar button to start a new match.

## Team

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/gennarocarmine.png" width="100px" alt=""/><br />
      <a href="https://github.com/gennarocarmine">GitHub</a>
    </td>
    <td align="center">
      <img src="https://github.com/lorenzo046.png" width="100px" alt=""/><br />
      <a href="https://github.com/lorenzo046">GitHub</a>
    </td>
  </tr>
</table>
