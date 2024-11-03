
## Description

This repository contains solutions and implementations for Lab #2 of the Neural Networks and Data Science course, covering LLM inference, performance analysis, Fibonacci sequences, and chaos theory.

## Problem Set Overview

### Problem 1: Local LLM Inference with llama.cpp

Implementation of local LLM inference using llama.cpp, including:
* Repository setup and compilation with CUDA support
* Model configuration and script setup
* Conversation implementation with Llama-3.1-8b
* Comparative analysis of different models' coding capabilities

### Problem 2: Performance Analysis

Investigation of token generation speed considering:
* Parameter impact analysis
* Thread count influence
* GPU layer effects
* Visualization of results using matplotlib

Configuration Table:

![table](https://github.com/user-attachments/assets/d960366a-2f49-428f-8636-ff5150104b53)

### Problem 3: Fibonacci Sequence Implementation

Implementation of the Fibonacci sequence defined as:
```
x(n+1) = x(n) + x(n-1)
```

Features:
* Initial sequence generation
* Large number handling (up to 10^7)
* Statistical analysis
* Visualization of number distribution

### Problem 4: Chaotic Systems Analysis

Study of the logistic iterator as a chaotic system:
```
x(n+1) = r x(n)(1 - x(n))
```

Features:
* Implementation of sequence generator
* Analysis of convergence properties
* Investigation of butterfly effect
* Visualization of chaotic behavior

## Installation

```bash
# Clone llama.cpp repository
git clone https://github.com/ggerganov/llama.cpp
cd llama.cpp

# Compile with CUDA support
make GGML_CUDA=1 -j 32

# Mount fileserver and copy files
mount /share
cp -r /share/llm .
cd llm
chmod +x llm.py
```

## Usage

Each problem has its own Jupyter notebook:
* `problem1_llm_analysis.ipynb`
* `problem2_performance_metrics.ipynb`
* `problem3_fibonacci.ipynb`
* `problem4_chaos_analysis.ipynb`

For large number handling in Problem 3, use:
```python
import sys
sys.set_int_max_str_digits(0)
```

## Dependencies

* Python 3.x
* CUDA toolkit
* matplotlib
* Jupyter Notebook

## Documentation

Each problem's implementation is documented in its respective notebook with:
* Detailed explanations
* Code implementation
* Results analysis
* Visualizations

## Support

For system monitoring:
* GPU monitoring: Use `nvtop`
* System monitoring: Use `btop`
