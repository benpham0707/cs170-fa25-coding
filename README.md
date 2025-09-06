# CS 170 Fall 2025 Coding Notebooks
Coding Jupyter Notebooks for Fall 2025 Iteration of CS 170.

## Local setup instructions with uv (recommended)

1. Install `uv` following the instructions [here](https://docs.astral.sh/uv/getting-started/installation/). 
2. Create a virtual environment (venv) using `uv venv --python 3.9`. 
3. Activate the environment: 
    - If on macOS/Linux: `source .venv/bin/activate`
    - If on Windows: `.venv\Scripts\activate`
4. Install jupyter: `uv pip install jupyter`.
5. Clone this repository: `git clone https://github.com/Berkeley-CS170/cs170-fa25-coding`.
6. If you ever want to switch to a different environment, simply run the command `deactivate`. 
7. Profit!!!

For all reasonable use cases, `uv` can be used as a drop in replacement for `pip` for Python environment management. It's way faster and has a very nice interface. There's a lot more to `uv` than venvs! You can read more about it [here](https://docs.astral.sh/uv/getting-started/).

## Instructions for completing each coding homework
1. Make sure that you've completed the initial local setup above. 
2. Open up your terminal
3. `cd` into your specific coding homework directory, e.g.:
    ```bash
    cd <wherever your homework lives>/cs170-fa25-coding/hw02
    ```
4. Make sure you've activated the venv: `source .venv/bin/activate` or `.venv\Scripts\activate` if on Windows.
5. Install all python package requirements for that homework:
    ```bash
    uv pip install -r requirements.txt
    ```
    or run the command in the notebook cell. If there isn't a `requirements.txt` file in the coding homework directory, you can skip this step.
6. Launch jupyter: `jupyter notebook` or `jupyter lab`. You can also use directly VSCode's built in ipynb UI, which is quite nice and featureful (in which case you won't even need to activate the venv, you'll be prompted to select the kernel for the notebook, and then pick the venv you created).
7. Navigate to the jupyter notebook for the assignment and complete it! Good luck :D
8. Once you're done, submit your completed `.ipynb` file to Gradescope, and if you want, deactivate 

## Local setup instructions if you're using conda (not recommended)
1. Install Anaconda following the instructions [here](https://www.anaconda.com/products/distribution).
2. Open up your terminal.
3. Create a conda environment (with python 3.9):
    ```bash
    conda create -n cs170 python=3.9
    ```
4. Activate the environment:
    ```bash
    conda activate cs170
    ```
5. Install pip:
    ```bash
    conda install pip
    ```
6. Install jupyter:
    ```bash
    conda install jupyter
    ```
7. Clone this repository somewhere in your device:
    ```bash
    git clone https://github.com/Berkeley-CS170/cs170-fa25-coding
    ```
8. Once you're done, deactivate the conda environment to return to your default environment:
    ```bash
    conda deactivate
    ```