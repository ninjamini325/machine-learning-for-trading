# Machine Learning for Trading (ML4T) - 2nd Edition

This project accompanies the book [Machine Learning for Algorithmic Trading](https://www.amazon.com/Machine-Learning-Algorithmic-Trading-alternative/dp/1839217715), 2nd Edition by Stefan Jansen. It demonstrates how machine learning (ML) techniques can be applied to develop, backtest, and evaluate algorithmic trading strategies using a broad range of data sources and ML models.

---

## Project Overview

ML4T covers practical applications of ML in trading, from data sourcing and feature engineering to model training and strategy backtesting. The project contains over 150 Jupyter notebooks that implement concepts and algorithms discussed in the book, providing hands-on examples for:

- Working with market, fundamental, and alternative data (including text and image data)
- Training and tuning ML models for return prediction and signal generation
- Designing and backtesting trading strategies driven by ML predictions
- Using advanced ML techniques including deep learning, reinforcement learning, and generative models

The notebooks are organized into thematic chapters covering foundational concepts, ML fundamentals, natural language processing, and deep & reinforcement learning.

---

## How It Works

The ML4T workflow is an end-to-end process for developing ML-driven trading strategies:

1. **Idea Generation & Data Collection**  
   Define an investment universe and collect relevant market, fundamental, and alternative data.

2. **Feature Engineering**  
   Extract informative features (alpha factors) from raw data using financial domain knowledge and ML techniques.

3. **Model Training & Optimization**  
   Train supervised or unsupervised ML models to predict asset returns or classify market regimes. Tune hyperparameters and evaluate predictive performance.

4. **Strategy Design & Backtesting**  
   Translate model predictions into trading signals and design portfolio construction rules. Backtest strategies using historical data with realistic market simulations.

5. **Evaluation & Iteration**  
   Analyze strategy performance, risk, and robustness. Iterate on data, features, models, and strategy design to improve results.

This workflow is demonstrated using Python libraries such as pandas, scikit-learn, TensorFlow, PyTorch, Zipline, and Backtrader.

---

## How to Use It

### Installation

The project requires Python 3.8 and various data science and finance libraries. We recommend using conda environments for dependency management.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ninjamini325/machine-learning-for-trading.git
   cd machine-learning-for-trading
   ```

2. **Create and activate a conda environment:**
   ```bash
   conda create -n ml4t python=3.8
   conda activate ml4t
   ```

3. **Install dependencies:**
   Use the OS-agnostic base environment file for latest compatible versions:
   ```bash
   mamba env update -n ml4t -f installation/ml4t-base.yml
   ```
   Alternatively, use OS-specific environment files in `installation/windows/`, `installation/linux/`, or `installation/macos/`.

4. **Download and preprocess data:**
   Follow instructions in the `data/README.md` and relevant notebooks to download market and alternative data sources.

5. **Run Jupyter notebooks:**
   Launch Jupyter Lab or Notebook from the project root:
   ```bash
   jupyter lab
   ```
   or
   ```bash
   jupyter notebook
   ```
   Open notebooks in the chapter directories to explore examples.

### Additional Notes

- Some notebooks require the `backtest` environment for Zipline backtesting (Python 3.6).
- GPU support for deep learning can be enabled by installing `tensorflow-gpu` in the environment.
- The project supports running in Docker containers for easier setup (see `installation/README.md`).

---

## Strategies Offered

The project covers a wide range of trading strategies and ML approaches, including:

- **Supervised Learning Strategies:**  
  Linear regression, logistic regression, random forests, gradient boosting machines for return prediction and classification.

- **Unsupervised Learning Strategies:**  
  Dimensionality reduction (PCA, ICA), clustering, and data-driven risk factors for portfolio construction.

- **Natural Language Processing (NLP):**  
  Sentiment analysis, topic modeling, and word embeddings applied to financial text data such as SEC filings and earnings calls.

- **Deep Learning Strategies:**  
  Feedforward neural networks, convolutional neural networks (CNNs) for time series and image data, recurrent neural networks (RNNs) for sequential data.

- **Generative Models:**  
  Generative adversarial networks (GANs) for synthetic time series data generation.

- **Reinforcement Learning:**  
  Deep Q-learning agents trained to optimize trading decisions in simulated market environments.

- **Backtesting and Portfolio Optimization:**  
  Event-driven and vectorized backtesting engines (Zipline, Backtrader), portfolio optimization using mean-variance and hierarchical risk parity.

---

## Community and Support

Join the ML4T community to discuss the book, code examples, and trading strategies:

- Online platform: [https://exchange.ml4trading.io/](https://exchange.ml4trading.io/)
- GitHub repository: [https://github.com/stefan-jansen/machine-learning-for-trading](https://github.com/stefan-jansen/machine-learning-for-trading)
- Raise issues or contribute improvements via GitHub.

---

## References

- Book website: [ml4trading.io](https://ml4trading.io)
- Book on Amazon: [Machine Learning for Algorithmic Trading](https://www.amazon.com/Machine-Learning-Algorithmic-Trading-alternative/dp/1839217715)

---

This README provides a comprehensive guide to understanding, installing, and using the ML4T project, as well as an overview of the strategies it offers.
