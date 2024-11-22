# SubGraph AutoEncoder (SGAE): A Framework for Link Prediction
This project introduces SGAE (SubGraph AutoEncoder), a novel framework for link prediction in graphs based on the Graph AutoEncoder (GAE) model. The proposed method enhances the standard GAE by incorporating subgraph extraction and subgraph embedding generation techniques.

## Overview
SGAE uses two key innovations:

### Subgraph extraction methods:
h-hop extraction: Extracts traditional h-hop subgraphs to capture local graph structures.
DIS (Dynamic Importance Sampling): A proposed method for adaptive subgraph extraction.
Subgraph embedding generation methods:

### Subgraph feature vector extraction methods:
NDP (Node Distance Penalty): A novel method that uses node distances to generate subgraph feature vectors.
CNN-based method: A method that applies convolutional neural networks (CNN) to the feature matrix of subgraphs to extract subgraph feature vectors.
These innovations are evaluated on four standard datasets (Karate, USAir Power, and Yeast) to demonstrate the effectiveness of the SGAE framework for link prediction.

## Project Structure
- `SGAE.ipynb`: Contains the full implementation of the SGAE framework, including:
- Subgraph extraction using h-hop and DIS.
- Subgraph feature vector generation using NDP and CNN-based methods.
- Link prediction and evaluation metrics.

## Evaluation Metrics
The performance of the SGAE framework is evaluated using the following metrics:

- Accuracy
- Recall
- Precision
- F1-Score
- Average Precision (AP)
- Precision-Recall AUC (PR-AUC)

## Results
The SGAE framework demonstrates significant improvements in link prediction accuracy across all datasets, particularly when employing the proposed subgraph extraction and embedding methods. The combination of DIS and NDP yields the highest overall performance, showcasing the potential of these methods for capturing localized graph structures effectively.

## Note
This framework builds upon the foundational concepts of GAE while introducing novel techniques for enhanced performance. Future work involves applying these methods to larger and more complex datasets for further validation.

## References
- Kipf, T.N., & Welling, M. (2016). Variational Graph Auto-Encoders. [Link to Paper](https://doi.org/10.48550/arXiv.1611.07308)
- Karami,vahidipour (2024). Link prediction framework using graph neural network based on subgraph‏. [Link to Paper](https://doi.org/10.22052/scj.2024.253458.1179)
