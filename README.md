### Project Setup Instructions

This guide will walk you through setting up a new Conda environment, installing necessary dependencies, and ensuring data files are correctly placed to run the notebook for the Resource-Constrained Project Scheduling Problem (RCPSP).

#### Step 1: Create a New Conda Environment

We recommend using Conda to manage your environments and dependencies. If you do not have Conda installed, please install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda](https://www.anaconda.com/products/individual).
<br>To create a new Conda environment, run the following command in your terminal:</br>

```sh
conda create -n rcpsp_env python=3.12.2
```
#### Step 2: Activate the Conda Environment
Activate the newly created environment with:
```sh
conda activate rcpsp_env
```
#### Step 3: Install Requirements Using pip
With your Conda environment activated, install the required Python packages listed in requirements.txt using pip:
```sh
pip install -r requirements.txt
```
Make sure requirements.txt is in the current directory where the command is run.

#### Step 4: Data Files Setup
Ensure that the following data files:
- pcm_execution_schedule.csv
- full_pcm_execution_schedule.csv
- limited_pcm_resources.csv
- full_pcm_resources.csv
are placed within a subdirectory called /data relative to the notebook's directory.

<br>Your directory structure should look like this:</br>
.
+-- data
|   +-- pcm_execution_schedule.csv
|   +-- full_pcm_execution_schedule.csv
|   +-- limited_pcm_resources.csv
|   +-- full_pcm_resources.csv
+-- EEC289Q_FinalProject_ProjectSchedule.ipynb
+-- requirements.txt

#### Step 5: Run the notebook
Now that the environment is set up and the data is in place, you can start the Jupyter notebook server:
```sh
jupyter notebook
```