Indexing on WideResNet model with SAM Optimizer for CIFAR-10 

This repository contains the implementation of WideResNet with Sharpness-Aware Minimization (SAM) optimizer for the CIFAR-10 dataset. The code is written in PyTorch and includes training, evaluation, and visualization of the model's performance.
Requirements:

    Python 3.7+
    PyTorch 1.8.0
    Torchvision 0.9.0
    Faiss 1.7.1
    Torchmetrics 0.11.0
    Matplotlib 3.4.2
    Numpy 1.21.0
    Pandas 1.3.0
    Scikit-learn 0.24.2

Usage

Install the required packages:


    pip install -r requirements.txt

    
Training

The training script supports various hyperparameters, including learning rate, batch size, depth, dropout, epochs, label smoothing, momentum, number of threads, rho, weight decay, and width factor. You can adjust these hyperparameters to train the model with different configurations.

Evaluation

The evaluation script calculates the precision and recall at k for the given model and dataset.

Visualization

The visualization script displays the query images and their nearest neighbors in the CIFAR-10 dataset using the Faiss index.

Indexing

The code includes two indexing methods: FlatL2 and IVFF (Inverted File with Flat Index). You can choose the desired indexing method by modifying the indexing_method variable in the visualization script.
License

This project is licensed under the MIT License - see the LICENSE file for details.
