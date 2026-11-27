# Assignment-4
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter elements of Matrix A:")
A = [[int(input(f"A[{i}][{j}]: ")) for j in range(cols)] for i in range(rows)]

print("Enter elements of Matrix B:")
B = [[int(input(f"B[{i}][{j}]: ")) for j in range(cols)] for i in range(rows)]

result = [[A[i][j] + B[i][j] for j in range(cols)] for i in range(rows)]

print("\nMatrix A:", A)
print("Matrix B:", B)
print("Addition of Matrix A and B:")
for row in result:
    print(row)
