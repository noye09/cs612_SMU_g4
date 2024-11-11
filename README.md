Backdoor Models Overview

This repository contains models trained with different backdoor attacks, triggers, and target classes. Below is an overview of each model and its corresponding characteristics.

Models 1 to 5

Each of these folders contains a backdoor model trained on different datasets and using different triggers and attack targets:

Model 1: Trained on the MNIST dataset.

Models 2-5: Trained on the CIFAR-10 dataset.

Models 6 and 7 (Week 4 Exercise)

Model 6: Trained on the MNIST dataset with a target class of 5, using 30 poisoned training samples.

Model 7: Trained on the MNIST dataset with a target class of 5, using 50 poisoned training samples.

Model 8 (Third-Party Backdoor Model)

Dataset: MNIST

Target Class: 0

Poisoned Data Source: Third-party GitHub repository.

Metrics:

Test Clean Accuracy (TCA): 0.9818

Attack Success Rate (ASR): 0.9995

Model 9 (Third-Party Backdoor Model)

Dataset: CIFAR-10

Target Class: 1

Poisoned Data Source: Third-party GitHub repository.

Metrics:

Test Clean Accuracy (TCA): 0.5163

Attack Success Rate (ASR): 0.9311

Reference: GitHub Repo - badnets-pytorch

Model Architectures

Models 8 and 9: Use badnet.py for their model architectures.

Models 1-7: The architectures can be found in model_cifar10.py and model_mnist.py located under the model_class folder.

Running the Models

To select a model to run, change the value of selected_model_options in the main script.

The models can be executed for multiple runs (set using number_of_runs), and the results will be merged and saved as a CSV file in the output folder.
