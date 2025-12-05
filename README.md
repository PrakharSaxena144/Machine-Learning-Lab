# Machine-Learning-Lab

A personal collection of Jupyter Notebook lab exercises and projects completed for the Machine Learning Lab course during 5th Semester, B.Tech (Artificial Intelligence). This repository contains all code, experiments, and short lab reports I completed between August 2025 and December 2025.

Repository goals
- Keep a reproducible, well-organized record of lab work and experiments.
- Make it easy to re-run notebooks and reproduce results locally or on Colab.
- Provide clear explanations, dataset notes, and references for each lab task.

Timeline
- Course period: Aug 2025 — Dec 2025
- Owner: GitHub user PrakharSaxena144 (https://github.com/PrakharSaxena144)

Contents
- Notebooks/ : Jupyter notebooks for each lab session or assignment.
- data/ : Datasets for notebooks (I will add datasets here).
- reports/ : Short write-ups, solved exercises, plots, or saved results.
- utils/ : Helper scripts or modules used across notebooks (if any).
- README.md : This file.
- requirements.txt : Python package list to reproduce the environment.
- .gitignore : Common files to ignore.

What I added just now
- A requirements.txt listing common ML packages so you can install dependencies quickly.
- README updates with usage instructions for VS Code Jupyter and Google Colab.
- A small data/README with dataset guidance and a .gitignore to keep the repo tidy.

Quick start — clone the repo
```bash
git clone https://github.com/PrakharSaxena144/Machine-Learning-Lab.git
cd Machine-Learning-Lab
```

Environment (recommended)
- Using conda:
```bash
conda create -n ml-lab python=3.10 -y
conda activate ml-lab
pip install -r requirements.txt
```
- Using pip + venv:
```bash
python -m venv .venv
source .venv/bin/activate   # on Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Running in VS Code (Jupyter file)
- Open the repo folder in VS Code.
- Install the Python and Jupyter extensions.
- Select the `ml-lab` interpreter you created and open the .ipynb notebook.
- Run cells or run the whole notebook through the Run toolbar.

Running in Google Colab
- If you want to run a notebook in Colab:
  1. Upload the notebook file to Colab or open it from GitHub (File → Open notebook → GitHub).
  2. Install any extra dependencies at the top of the notebook (Colab already has many preinstalled). Example to install from this repo's requirements:
```python
!pip install -r https://raw.githubusercontent.com/PrakharSaxena144/Machine-Learning-Lab/main/requirements.txt
```
  3. If your notebook uses local datasets, upload them to Colab or mount your Google Drive:
```python
from google.colab import drive
drive.mount('/content/drive')
```
  4. Update dataset paths in the notebook to point to the mounted Drive path or the uploaded file location.

Datasets
- I'll add datasets under the `data/` folder in this repo (one dataset per notebook or organized by lab).
- For large datasets (>50–100 MB) consider using Git LFS or storing them in Google Drive and linking in the notebook. See data/README.md for guidance.

requirements.txt
- A curated list of packages used across the notebooks is provided in requirements.txt. Install with:
```bash
pip install -r requirements.txt
```
- If you want pinned versions for exact reproducibility, I can generate a requirements file with version pins (pip freeze) — tell me if you'd like that.

Notebook conventions used
- Each notebook begins with title, author (GitHub handle), date, and objective.
- Typical sections: Data → Preprocessing → Modeling → Evaluation → Conclusions.
- Random seeds are set where applicable for reproducibility.

Reproducibility tips
- Use the same Python minor version (Python 3.10 recommended).
- Seed random generators (numpy, sklearn, torch/tensorflow).
- Record library versions when results are sensitive to implementation.

Contributing
- This is primarily a personal lab-record repository, but suggestions are welcome — open an issue or PR.
- If you contribute a notebook, follow the notebook conventions and add a short description to the filename.

License
- If you want this repo to be reusable, add a LICENSE file (MIT is a common choice). Tell me if you'd like me to add one.

Contact
- GitHub: https://github.com/PrakharSaxena144

Acknowledgements
- Course instructors and lab TAs.
- Open-source libraries used (numpy, pandas, scikit-learn, matplotlib, seaborn, etc.).
