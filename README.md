# DT-NIDS Evasion Attacks

## Project Overview
This repository, focuses on exploring evasion and poisoning attacks on a decision-tree-based network intrusion detection system (NIDS). The project builds upon a [baseline decision tree (DT) model](https://github.com/tamerthamoqa/cic-ids-2018-intrusion-detection-classification/blob/master/trained_models/decision-tree-classifier.pkl) provided by [cic-ids-2018-intrusion-detection-classification](https://github.com/tamerthamoqa/cic-ids-2018-intrusion-detection-classification) and extends it to study and implement evasion and poisoning attacks. The work includes experiments targeting both benign and malicious traffic, along with an analysis of feature importance and relationships to inform effective evasion strategies. The project also involves retraining the model to classify four distinct types of traffic: benign, bot, DoS-Hulk, and DoS-SlowHTTPTest.

## Table of Contents
- [Project Overview](#project-overview)
- [Repository Structure](#repository-structure)
- [Acknowledgements](#acknowledgements)

## Repository Structure
The repository contains the following directories and files:

- **`notebooks/`**
  - **`evasion_attack_benign_samples.ipynb`**: A notebook testing evasion strategies on benign samples.
  - **`evasion_attacks_bot_samples.ipynb`**: A comprehensive notebook containing experiments, successful and unsuccessful evasion attempts, and dataset/feature analyses for bot attacks.
  - **`poisoning_attack.ipynb`**: A notebook demonstrating the effects of poisoning the training data on the model's performance.
  - **`model_with_attack_names/`**: Contains notebooks that goes through each steps of Preparation, Training and Testing that shows sucessful evasion attack for DoS-SlowHTTPTest attack.
    - **`1-Preparing_Datasets.ipynb`**: Prepares datasets for training and testing.
    - **`2-Training_Decision_Tree.ipynb`**: Trains a decision tree model to classify four traffic classes.
    - **`3-Testing.ipynb`**: Tests the trained model on unseen data.

## Acknowledgements
Special thanks to Tamer Thamoqa for making their implementation publicly available. Their detailed documentation and well-organized repository greatly facilitated our understanding and replication of their results!

---

This project is part of the **INSE 6120 (Fall 2024)** course at Concordia University.
