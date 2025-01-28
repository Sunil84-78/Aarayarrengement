def perform_operation(arr, start_index, end_index, value):
    for i in range(start_index - 1, end_index):
        arr[i] += value
    return arr


arr = [0,0,0,0,0]
start_index = int(input("Enter the start index for Operation 1 (1-based index): "))
end_index = int(input("Enter the end index for Operation 1 (1-based index): "))
value = int(input("Enter the value to add for Operation 1: "))
arr = perform_operation(arr, start_index, end_index, value)
print(f"After Operation 1: {arr}")

start_index = int(input("Enter the start index for Operation 2 (1-based index): "))
end_index = int(input("Enter the end index for Operation 2 (1-based index): "))
value = int(input("Enter the value to add for Operation 2: "))
arr = perform_operation(arr, start_index, end_index, value)
print(f"After Operation 2: {arr}")

start_index = int(input("Enter the start index for Operation 3 (1-based index): "))
end_index = int(input("Enter the end index for Operation 3 (1-based index): "))
value = int(input("Enter the value to add for Operation 3: "))
arr = perform_operation(arr, start_index, end_index, value)
print(f"After Operation 3: {arr}")

max_value = max(arr)
print(f"The maximum value in the final array is: {max_value}")
