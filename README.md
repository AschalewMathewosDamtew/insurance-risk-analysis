# Task 2: Data Version Control (DVC) Setup

## Overview
This branch focuses on implementing Data Version Control (DVC) for tracking dataset changes in the insurance risk analysis project. The objective is to establish a robust versioning system for our dataset, ensuring that data changes are properly managed and recorded.

## Tasks Completed
- **DVC Installation**: Installed DVC in the project environment.
- **DVC Initialization**: Initialized DVC in the project directory using `dvc init`.
- **Local Remote Storage Configuration**:
  - Created a local storage directory for dataset versioning.
  - Configured the local storage as a DVC remote.
- **Data Tracking**:
  - Added the dataset (`dataset.csv`) to DVC for version control.
- **Version Control Management**:
  - Committed changes to Git, including DVC tracking files.
  - Pushed data to the local remote storage.

## Steps to Reproduce
1. Install DVC:
   ```bash
   pip install dvc
2. Initialize DVC:
   ```bash
   dvc init
3. Set up Local Remote Storage:
   ```bash
   dvc remote add -d localstorage /path/to/your/local/storage
4. Add Dataset to DVC
   ```bash
   dvc add dataset.csv
5. Stage and Commit Changes:
   ```bash
   git add dataset.csv.dvc .gitignore
   git commit -m "Track Dataset with DVC"
6. Push Data to Local Remote
   ```bash
   dvc push

This README serves as a guide for understanding the setup and processes related to DVC in this branch. Please refer to the main branch for additional tasks and overall project context.