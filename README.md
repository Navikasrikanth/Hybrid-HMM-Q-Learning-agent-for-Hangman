Hybrid HMM-RL Hangman Agent 🎯

This repository contains the implementation of a Hybrid Hidden Markov Model (HMM) and Reinforcement Learning (RL) agent designed to solve the classic Hangman word-guessing game. The model combines probabilistic inference and reward-based learning to improve prediction accuracy and win rate across training episodes.

-> Project Overview

Goal: Develop an intelligent Hangman player that learns optimal guessing strategies through experience.

Techniques Used:

Hidden Markov Model (HMM): Predicts letter probabilities based on observed patterns.

Reinforcement Learning (RL): Optimizes guesses via Q-learning and reward feedback.

Dataset: Custom word corpus located in data/corpus.txt.

-> Features

Preprocessing pipeline for cleaning and grouping vocabulary by length.

HMM for probability estimation of letter occurrences.

Q-learning for adaptive decision-making and exploration vs. exploitation balance.

Configurable training parameters such as epsilon decay, alpha (learning rate), and reward structure.

-> Model Design Highlights

State: Represents current game progress and known letters.

Action: Choosing the next letter to guess.

Reward: Positive for correct guesses, negative for incorrect ones.

Exploration Strategy: Epsilon-greedy with decay to ensure learning stability.

-> Files Included

Final_ML_Model.ipynb — Main implementation notebook.
corpus.txt - training dataset
data.txt - test dataset
README.md — This documentation file.

How to Run

Clone the repository:

git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>


Open Final_ML_Model.ipynb in Google Colab or Jupyter Notebook.

Ensure your dataset is in the data/ folder.

Run all cells to train and evaluate the model.

-> Results

Achieved improved win rate and prediction accuracy through combined HMM-RL approach.

Observed significant learning stabilization over training epochs.
