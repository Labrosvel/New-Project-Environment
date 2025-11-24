# 🧩 End‑to‑End Process for a New Project
## 1. Create the Repo & Structure
   ### On GitHub (or locally, then push):
        Create a new repo: my-project-name
        Clone it locally: git clone https://github.com/yourusername/my-project-name.git
			  cd my-project-name
   ### Inside the repo, set up a clean folder structure:
	my-project-name/
	├── notebooks/        # Jupyter notebooks
	├── src/              # Python source code
	├── data/             # Raw/processed datasets (ignored in git)
	├── models/           # Saved models (ignored in git)
	├── environment.yml   # Conda environment file
	├── .gitignore
	└── README.md

## 2. Copy or Create Your Notebook
   - Place your first notebook (from the web or scratch) under notebooks/.
   - Commit it

## 3. Set Up Conda Environment
   ### Create a new environment:
    	conda create -n my-project-env python=3.10
		conda activate my-project-env
   ### Install JupyterLab:
    	conda install -c conda-forge jupyterlab ipykernel
   ### Register kernel:
    	python -m ipykernel install --user --name=my-project-env --display-name "Python (my-project-env)"

## 4. Run Notebook Locally
   ### - Launch JupyterLab from repo root:
       jupyter lab
   ### - Open notebooks/my_notebook.ipynb and select kernel Python (my-project-env).

## 5. Add Dependencies
   ### - Install packages as needed (pip install or conda install).
   ### - Export environment:
    	conda env export > environment.yml
        → This captures both conda and pip packages.

## 6. Keep Repo Clean
   ### Add  .gitignore:
    		.ipynb_checkpoints/
			__pycache__/
			data/
			models/
			*.log
   ### Commit it:
    		git add .gitignore
			git commit -m "Add gitignore for checkpoints, data, models"
			git push origin main

## 7. Reproducibility

    Anyone (or future you) can recreate the environment:
    	conda env create -f environment.yml
    Update env when new packages are added:
    	conda env update -f environment.yml --prune

🔄 Your Repeatable Checklist
    1. Repo + structure
    2. Notebook in notebooks/
    3. Conda env + JupyterLab + kernel
    4. Run notebook locally
    5. Install packages → export env
    6. .gitignore cleanup
    7. Commit + push everything
