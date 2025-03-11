# mmadness-2025

Dataset description (and download): https://www.kaggle.com/competitions/march-machine-learning-mania-2025/data

Nate Silver's 2024 odds (download these and put in the same folder as above, just for fun): https://www.kaggle.com/datasets/tztang/ml-mania-2024

1. Make a virtual environment (add to gitignore if needed)

2. Install requirements

3. (mac-specific) if you get a weird python 32-bit version error, in a terminal OUTSIDE THE VIRTUAL ENVIRONMENT, run the following (and restart your vscode terminal):

```
brew install libomp
```

***Run the following IN ORDER***


**2025_notebook.ipynb**

- 2025_notebook contains the current strategy, heavily based on the 2023 winner's gradient-boosted random forest
- Make sure to skim the notebook and update years where necessary (find the 2025s and change to the updated year, etc).
- If data formatting gets changed by Kaggle, this will break.
- Just running this file is sufficient for creating a kaggle-style submission for the march machine learning mania competition (as of 2025)

**simulate_n_brackets.ipynb**

- simulate-n-brackets contains the logic to create simulated brackets by using the probabilities generated in submission.csv as weighted coin flips
- It also generates and saves a (currently slightly odd-looking) visual representation of one bracket

**simulated-bracket-playground**

- Check it out! Contains some fun stuff that can be done with the simulated brackets stored in bracket_simulations.csv


Code to simulate n brackets using previous years' submission format: https://www.kaggle.com/code/lennarthaupts/simulate-n-brackets/notebook