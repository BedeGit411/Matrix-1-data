# Matrix-1-data
A code Identifying 2 by 2 matrix
def are_matrices_identical(matrix1, matrix2):
    if len(matrix1) != 2 or len(matrix2) != 2 or len(matrix1[0]) != 2 or len(matrix1[1]) != 2 or len(matrix2[0]) != 2 or len(matrix2[1]) != 2:
        return False  # Matrices are not 2x2

    for i in range(2):
        for j in range(2):
            if matrix1[i][j] != matrix2[i][j]:
                return False  # Matrices are not identical
    return True  # Matrices are identical

# Example matrices
matrix_a = [[1, 2], [3, 4]]
matrix_b = [[1, 2], [3, 4]]

if are_matrices_identical(matrix_a, matrix_b):
    print("Matrices are identical")
else:
    print("Matrices are not identical")
