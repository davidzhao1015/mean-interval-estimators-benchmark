# 📊 Confidence Interval Benchmarking for Skewed Data

This project benchmarks methods for estimating **confidence intervals (CIs) for the mean** in **right-skewed, overdispersed data**, simulating hospital length of stay (LOS) distributions for rare diseases.

It compares:
- **t-distribution method**
- **z-distribution method**
- **Bootstrap percentile method**

Benchmarking is done via simulation to evaluate:
- **Coverage probability** (does the CI include the true mean?)
- **Interval width** (how wide is the CI?)

---

## 📝 Motivation

Hospital length of stay data, especially in rare diseases like autoimmune encephalitis, often exhibit **right-skewness** and **high variability** (overdispersion).  
This notebook examines how different CI methods perform under these challenging conditions, helping analysts choose appropriate methods for small, skewed samples.

---

## 🧪 Methods Overview
1. **Simulate skewed population data** using log-normal distributions.
2. **Draw random samples** of varying sizes (n = 10, 30, 100).
3. **Compute CIs** using t-distribution, z-distribution, and bootstrap methods.
4. **Assess performance** by coverage probability and average CI width.
5. **Visualize results** with bar plots.

---

## 📂 Repository Structure
/ (root)  
├── interval-estimate-mean-benchmark.ipynb   # Main notebook  
├── requirements.txt                         # Project dependencies (numpy, scipy, pandas, seaborn, matplotlib, tqdm)  
├── README.md                                # Project description & usage guide  

---

## 🚀 How to Run This Notebook

### 🟢 Option 1: Run in Binder (no install needed)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/davidzhao1015/mean-interval-estimators-benchmark/HEAD?urlpath=%2Fdoc%2Ftree%2Finterval-estimate-mean-benchmark_20250509_DZ.ipynb)

### 🖥️ Option 2: Run Locally
1. Clone the repo:
    ```bash
    git clone https://github.com/davidzhao1015/mean-interval-estimators-benchmark
    cd mean-interval-estimators-benchmark
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Launch the notebook:
    ```bash
    jupyter notebook interval-estimate-mean-benchmark.ipynb
    ```

---

## 📊 Example Outputs
- Coverage Probability Comparison by Method, Sample Size, and Skewness
- Average Confidence Interval Width Visualization
- Observations on method accuracy & precision trade-offs

---

## ✅ Key Findings
- **t-distribution CIs** maintain better coverage in small, skewed samples (more conservative).
- **Bootstrap CIs** are narrower but tend to under-cover in small, highly skewed data.
- Differences across methods decrease as sample size increases.

---

## 📬 Contact
Xin (David) Zhao  
[GitHub](https://github.com/davidzhao1015)

---