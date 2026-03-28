# Python Scripting: The Bridge to Intelligence

*——high-level agility for low-level minds* 🕸️

While C/C++ handles the "how," Python handles the "what." In my workflow, Python serves as the essential glue for **Deep Learning**, **3D Computer Vision research**, and automating the mundane parts of site maintenance.

## 📝 To-Do List

- [x] **PyTorch Foundations**: Tensors, Autograd, and building Neural Networks.
- [ ] **Data Science Stack**: Mastering `NumPy`, `Matplotlib`, and `OpenCV`.
- [ ] **Automation**: Scripting MkDocs deployments and file organization.
- [ ] **Blender API**: Scripting 3D scene generation for synthetic data.

------

## 💡 The Research Utility

## 1. Prototyping Speed

Python is the sandbox where ideas for **Gaussian Splatting** or **Spatial Intelligence** are tested before they are optimized in C++.

## 2. Deep Learning Ecosystem

From `torch` to `diffusers`, Python is the gateway to the state-of-the-art. I use it to implement papers and evaluate pre-trained models.

## 3. Clean & Functional

I aim for PEP 8 compliance and favor functional approaches (list comprehensions, map/filter) to keep scripts concise and readable.

------

## 🏗️ Core Libraries

| **Library**  | **Purpose**                    | **Status** |
| ------------ | ------------------------------ | ---------- |
| **NumPy**    | Linear Algebra & Array ops     | 🌕 Mastered |
| **PyTorch**  | Neural Rendering / CV Research | 🌗 Learning |
| **OpenCV**   | Image Processing & Calibration | 🌗 Learning |
| **Requests** | Web Scraping & API Interaction | 🌕 Mastered |

------

## 📂 Workflow Snippets

Python

```
import torch

# Simple Linear Layer in PyTorch
class SimpleNet(torch.nn.Module):
    def __init__(self):
        super().__init__()
        self.fc = torch.nn.Linear(3, 1) # 3D coord to 1D intensity

    def forward(self, x):
        return torch.sigmoid(self.fc(x))
```

------

## 🌐 External Resources

## 📖 Literature & Docs

- **Python Crash Course (Eric Matthes)**: Great for quick syntax refreshing.
- **Dive into Deep Learning (d2l.ai)**: An interactive guide to the math and code of AI.

## 🛠️ Environment

- **Package Manager**: `conda` / `mamba` for isolated research environments.
- **Interactive**: `Jupyter Notebooks` for quick experiments and visualization.

------

<p align="center">

<small>"Python is executable pseudocode." — Bruce Eckel</small>

</p>
