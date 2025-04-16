A = [
    [4, 6, 7, 7, 5],
    [3, 8, 9, 2, 6],
    [7, 1, 4, 8, 2],
    [5, 9, 3, 6, 7],
    [8, 2, 5, 4, 9]
]
B = [
    [6, 2, 9, 4, 7],
    [3, 8, 1, 5, 2],
    [9, 4, 7, 3, 8],
    [2, 5, 6, 9, 1],
    [7, 3, 2, 8, 4]
]

C = [[0 for _ in range(5)] for _ in range(5)]

for i in range(5):
    for j in range(5):
        for k in range(5):
            C[i][j] += A[i][k] * B[k][j]

print("Matriks A:")
for baris in A:
    print(baris)

print("\nMatriks B:")
for baris in B:
    print(baris)

print("\nHasil A x B:")
for baris in C:
    print(baris)
