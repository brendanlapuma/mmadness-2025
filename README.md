# mmadness-2025

Dataset description (and download): https://www.kaggle.com/competitions/march-machine-learning-mania-2024/data

1. Make a virtual environment (add to gitignore if needed)

2. Install requirements

3. (mac-specific) if you get a weird python 32-bit version error, in a terminal OUTSIDE THE VIRTUAL ENVIRONMENT, run the following (and restart your vscode terminal):

```
brew install libomp
```


**Explanation of strategies**

1. 2024 4th Place

- Entirely based on Nate Silver's odds (see the men's and women's excel files mentioned in his leaderboard submission)
- Employs goto conversion on those odds (a smart math thing that makes the odds more accurate), and simulates 10,000 brackets using weighted coin flips based on those odds

2. 2023 1st place
- Uses gradient-boosted decision trees (actually training a model)
- Generates every possible matchup in all of cbb (which was the submission format for that year)