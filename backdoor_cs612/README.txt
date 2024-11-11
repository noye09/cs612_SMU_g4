This repository contains models trained with different backdoor attacks, triggers, and target classes. Below is a summary of each model.
neural_cleanse_v2.ipynb is a backdoor detection model uisng neural clease method.

Models 1 to 5: 
- Model 1: Trained on MNIST.
- Models 2-5: Trained on CIFAR-10.

Models 6 and 7 (Week 4 Exercise):
- Model 6: MNIST, target class 5, 30 poisoned samples.
- Model 7: MNIST, target class 5, 50 poisoned samples.

Model 8 (Third-Party):
- Dataset: MNIST, Target Class: 0
- Source: Third-party GitHub
- TCA: 0.9818, ASR: 0.9995

Model 9 (Third-Party):
- Dataset: CIFAR-10, Target Class: 1
- Source: Third-party GitHub
- TCA: 0.5163, ASR: 0.9311
- Reference: badnets-pytorch (https://github.com/verazuo/badnets-pytorch.git)

Model Architectures:
- Models 8 and 9: Use badnet.py
- Models 1-7: Use model_cifar10.py and model_mnist.py under model_class folder

Running the Models:
- Select a model by changing selected_model_options in the main script.
- Execute multiple runs by setting number_of_runs. Results are saved as CSV in the output folder.

For further details, refer to the relevant files in this repository.

