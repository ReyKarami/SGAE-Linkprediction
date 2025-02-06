# SubGraph AutoEncoder (SGAE): A Framework for Link Prediction
This project introduces SGAE (SubGraph AutoEncoder), a novel framework for link prediction in graphs based on the Graph AutoEncoder (GAE) model. The proposed method enhances the standard GAE by incorporating subgraph extraction and subgraph embedding generation techniques.

## Overview
SGAE uses two key innovations:

### Subgraph Extraction Methods:
- h-hop extraction: Extracts traditional h-hop subgraphs to capture local graph structures and node relationships.
- DIS (Distance-based): A proposed method for subgraph extraction, selecting subgraphs based on the distance between feature vectors of subgraph nodes and those of target nodes.
### Subgraph Embedding Generation Methods:
- CNN-based feature extraction: Convolutional Neural Networks (CNN) are used to extract feature vectors from subgraphs.
- NDP (Normal Distance Penalty): This method introduces a novel approach to weighting nodes in subgraphs. It weighs the feature vectors of subgraph nodes to generate a more meaningful subgraph feature vector.

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
