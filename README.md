# 🧪 Run Jupyter Notebook with a Virtual Environment

This guide helps you configure and run Jupyter Notebooks inside a Python virtual environment (`venv`).



## 🚀 Getting Started

1. **Fork this repository** to your own GitHub account.
2. **Clone your fork** to your local machine:

   ```bash
   git clone https://github.com/YOUR_USERNAME/ai-agent-workshop.git
   cd ai-agent-workshop
   ```

3. **Activate Your Virtual Environment**

   ```bash
   python3 -m venv .venv
   source ./.venv/bin/activate
---

4. **Install Jupyter in the Virtual Environment**

Make sure Jupyter and IPython kernel support are installed **inside** the virtual environment:

```bash
pip install jupyter ipykernel
```

---

5. **Add the Virtual Environment to Jupyter as a Kernel**

Register your virtual environment with Jupyter so it appears as a kernel option:

```bash
python -m ipykernel install --user --name=myenv --display-name "Python (myenv)"
```

- `--name`: internal name for the kernel  
- `--display-name`: the name shown in the Jupyter interface

---

6. **Launch Jupyter Notebook**

Still inside the activated virtual environment, launch Jupyter Notebook:

```bash
jupyter notebook
```

Then, in the Notebook UI, select your kernel from:

```
Kernel → Change kernel → Python (myenv)
```

---

✅ You're all set! You can now work with isolated environments in Jupyter with full control.
