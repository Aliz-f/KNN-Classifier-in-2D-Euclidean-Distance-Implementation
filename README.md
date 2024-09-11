# K-Nearest Neighbors (KNN) Classifier in 2D

This repository contains a Python implementation of a **K-Nearest Neighbors (KNN)** classifier for 2D data points using the **Euclidean distance metric**. The classifier determines the class of query points based on the nearest neighbors from a provided dataset.

## Features

- Implements KNN classification in 2D.
- Supports any number of neighbors (`k`).
- Utilizes Euclidean distance for nearest neighbor search.
- Tested on the provided dataset `H3Data.mat`.

## Dataset

The provided dataset (`H3Data.mat`) includes:
- **Datamat**: A matrix where the first two columns represent the x and y coordinates, and the third column represents the class label of the points.
- **Querymat**: A matrix where the first column contains the x coordinates and the second column contains the y coordinates of the points to be classified.

## Implementation Details

The KNN function receives the following parameters:

1. `datamat`: A matrix containing the coordinates and class labels of the points.
2. `querymat`: A matrix containing the coordinates of the query points to classify.
3. `k`: The number of nearest neighbors to consider for the classification.

The function computes the Euclidean distance between each query point and the points in the dataset. Based on the `k` nearest neighbors, the function predicts the class for each query point using a majority vote.

## How to Run the Code

1. Clone the repository:
    ```bash
    git clone https://github.com/Aliz-f/KNN-Classifier-in-2D-Euclidean-Distance-Implementation.git
    ```

2. Install required libraries (if applicable):
    ```bash
    pip install -r requirements.txt
    ```

3. Run the `knn.ipynb` notebook to test the KNN classifier on the provided dataset.

## Usage Example

In the Jupyter notebook, the KNN function is used as follows:

```python
# Define k (number of neighbors)
k = 3

# Call the KNN classifier
predicted_classes = knn(datamat, querymat, k)

# Output the predicted classes for the query points
print(predicted_classes)
```

## Results

The KNN classifier was tested with \( k = 3 \) on the `H3Data.mat` dataset. The predicted classes for the query points were found to be [ ... ].
