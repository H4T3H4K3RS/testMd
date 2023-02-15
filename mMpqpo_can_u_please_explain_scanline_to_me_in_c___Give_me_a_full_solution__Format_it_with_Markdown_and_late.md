

# **Scanline Algorithm in C++**

The Scanline Algorithm is a technique used to fill in the interior regions of a closed polygon. It is used in computer graphics to convert a set of boundary lines into a two-dimensional shape. In this algorithm, each scanline is scanned from left to right and the intersection points of the polygon are determined. The pixels between the points are then filled in.

## **Algorithm**

1. Create a list of edges sorted by their y-coordinates.
2. Initialize a new empty list of active edges
3. Initialize the scanline y to the minimum y-coordinate of polygon
4. Fill in the pixels between the intersection points of all the active edges at the scanline y
5. For each edge in the edge list:
    * If the edge's minimum y-coordinate is equal to the scanline y, add it to the active edge list
    * If the edge's maximum y-coordinate is equal to the scanline y, remove it from the active edge list
6. Sort the active edge list by their x-coordinates
7. Increment the scanline y
8. Go back to Step 4 until the scanline y is greater than the maximum y-coordinate of the polygon

## **Mathematical Representation**

Let the coordinates of the vertices of the polygon be:

$V = \{(x_1, y_1), (x_2, y_2), (x_3, y_3), ..., (x_n, y_n)\}$

The scanline algorithm is used to fill the area inside the polygon. The steps of the algorithm can be represented mathematically as follows:

1. Create a list of edges sorted by their y-coordinates:

$E = \{(x_1, y_1, x_2, y_2), (x_2, y_2, x_3, y_3), ..., (x_n, y_n, x_1, y_1)\}$

2. Initialize a new empty list of active edges:

$A = \emptyset$

3. Initialize the scanline y to the minimum y-coordinate of polygon:

$y = min(y_1, y_2, y_3, ..., y_n)$

4. Fill in the pixels between the intersection points of all the active edges at the scanline y:

$P = \{(x_i, y) \mid \exists (x_i, y_i, x_j, y_j) \in A \text{ and } y_i \leq y \leq y_j\}$

5. For each edge in the edge list:
    * If the edge's minimum y-coordinate is equal to the scanline y, add it to the active edge list:

$A = A \cup \{(x_i, y_i, x_j, y_j) \mid y_i = y\}$

    * If the edge's maximum y-coordinate is equal to the scanline y, remove it from the active edge list:

$A = A \setminus \{(x_i, y_i, x_j, y_j) \mid y_j = y\}$

6. Sort the active edge list by their x-coordinates:

$A = \text{sort }A \text{ by } x_i$

7. Increment the scanline y:

$y = y + 1$

8. Go back to Step 4 until the scanline y is greater than the maximum y-coordinate of the polygon:

$y \leq max(y_1, y_2, y_3, ..., y_n)$