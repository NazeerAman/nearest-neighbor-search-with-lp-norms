# nearest-neighbor-search-with-lp-norms

**Introduction**
This code implements a Python function for finding the nearest neighbors in a dataset using various distance metrics (Lp-norms). It calculates the distance between two data points and returns an array containing pairs of closest points.

**Dependencies**
numpy (for efficient numerical operations)
matplotlib.pyplot (optional, for visualization)

**Installation**
If you haven't already, install the required libraries using pip:
*Bash*
pip install numpy matplotlib
Use code with caution.

**Code Structure**
The code consists of two primary functions:
calculate_distance(p1, p2, norm):
Takes two vectors (p1 and p2) and a norm identifier (1, 2, or np.inf) as input.
Calculates the distance between the vectors based on the specified norm:
L1 norm (Manhattan distance): sum of absolute differences.
L2 norm (Euclidean distance): square root of the sum of squared differences.
L-infinity norm (Chebyshev distance): maximum absolute difference.
Raises a ValueError for invalid norm values.
nearest_neighbors(array1, array2, norm):
Takes two NumPy arrays (array1 and array2) and a norm identifier (norm) as input.
Finds the nearest neighbor for each data point in array1 within array2 using the specified norm.
Returns a list of tuples, where each tuple represents a nearest neighbor pair.
