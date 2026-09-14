# Matrix-Decomposition-PCA-SVD
Comparison of PCA (Eigen-Decomposition) and SVD for image compression, including execution time, compressed size, and reconstruction quality.


# PCA vs SVD Image Compression

This project compares **PCA (Eigen-Decomposition)** and **Singular Value Decomposition (SVD)** for image compression and reconstruction.

## Project Objectives

* Apply Eigen-Decomposition/PCA to image compression.
* Apply SVD to image compression.
* Compare reconstruction quality using different numbers of components.
* Compare execution time and compressed file size.
* Visualize the principal components of an image.

## Methods Compared

| Aspect                 | Eigen-Decomposition / PCA | SVD            |
| ---------------------- | ------------------------- | -------------- |
| Decomposition          | Covariance matrix         | Direct SVD     |
| Numerical Stability    | Moderate                  | High           |
| Memory Usage           | Higher                    | Lower          |
| Large Images           | Less efficient            | More efficient |
| Execution Time         | 0.0735 seconds            | 0.0497 seconds |
| Compressed Size (100)  | 197.80 KB                 | 189.79 KB      |
| Reconstruction Quality | Good                      | Excellent      |

## Results

SVD performed better in terms of computational efficiency. It completed the decomposition in **0.0497 seconds**, compared with **0.0735 seconds** for Eigen-Decomposition.

SVD also produced a smaller reconstructed image file at **189.79 KB**, compared with **197.80 KB** using Eigen-Decomposition.

Overall, the results show that **SVD is faster and more computationally efficient** for this image compression experiment.

## Files

* `Matrix_Decomposition_PCA_SVD.ipynb` — Main Jupyter/Google Colab notebook.
* `bird.jpg` — Image used for PCA and SVD compression.
* `smile.jpg` — Image used for principal component visualization.

## Technologies

* Python
* NumPy
* Matplotlib
* Pillow
* Google Colab / Jupyter Notebook

## How to Run

1. Download or clone this repository.
2. Open `Matrix_Decomposition_PCA_SVD.ipynb` using **Google Colab** or **Jupyter Notebook**.
3. Make sure `bird.jpg` and `smile.jpg` are in the same directory as the notebook.
4. Run the notebook cells to reproduce the results.
