# Python-PyToarch
A learning-focused PyTorch repository where I explore deep learning fundamentals, build models, and experiment with neural networks.

## 🔧 Environment Setup (Important)

To run this project correctly, **Python 3.10 is required**.
Newer Python versions (like 3.12 or 3.13) may cause PyTorch installation issues.

### ✅ Step 1: Install Python 3.10

Download and install **Python 3.10 (64-bit)** from the official Python website.
During installation, make sure to check **“Add Python to PATH”**.

### ✅ Step 2: Create and activate virtual environment

```bash
python -m venv venv
venv\Scripts\activate
```

### ✅ Step 3: Upgrade pip

```bash
python -m pip install --upgrade pip
```

### ✅ Step 4: Install PyTorch with CUDA support (NVIDIA GPU)

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
```

> ⚠️ **Note:**
>
> * This command is for systems with an **NVIDIA GPU** and **CUDA 12.1 compatible drivers**
> * For CPU-only systems, install without the CUDA index URL

### ✅ Step 5: Verify installation

```python
import torch
print(torch.__version__)
print(torch.cuda.is_available())
```

If `torch.cuda.is_available()` returns **True**, your setup is successful ✅
