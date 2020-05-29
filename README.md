# Kth-largest-term
def largest_number(arr):
    for j in range(len(arr)):
        for i in range(len(arr) - 1):
            if arr[i] > arr[i + 1]:
                temp = arr[i + 1]
                arr[i + 1] = arr[i]
                arr[i] = temp
    return arr


k = int(input(print("Which largest term ?")))
arr = [3, 4, 7, 8, 1, 2, 5, 6, 9, 10]
result = (largest_number(arr))
print(result)
print(arr[-k])
