# Project Setup and Running Instructions

## Setting up the Virtual Environment

1. Activate the virtual environment:
   - On Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - On Unix/MacOS:
     ```bash
     source .venv/bin/activate
     ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Running Jupyter Notebook

1. Make sure your virtual environment is activated (you should see `(.venv)` in your terminal prompt)

2. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Your default web browser should open automatically with the Jupyter interface. If it doesn't, you can copy and paste the URL that appears in your terminal.

4. Navigate to and open the `ASD-Analysis.ipynb` notebook to start working.

## Deactivating the Virtual Environment

When you're done working, you can deactivate the virtual environment by running:
```bash
deactivate
``` 