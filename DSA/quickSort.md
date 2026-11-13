int partition(int arr[], int low, int high) {
    int pivot = arr[high];
    int i = low - 1;

    for (int j = low; j < high; j++) {
        if (arr[j] < pivot) {
            i++;
            swap(arr[i], arr[j]);
        }
    }

    swap(arr[i + 1], arr[high]);

    return i + 1;
}
## quick sort main function
void quickSort(int arr[], int low, int high) {
    if (low < high) {
        int p = partition(arr, low, high);

        quickSort(arr, low, p - 1);
        quickSort(arr, p + 1, high);
    }
}

Property	Quick Sort
Technique	Divide and Conquer
Best time	O(n log n)
Average time	O(n log n)
Worst time	O(n²)
Auxiliary partition space	O(1)
Average recursion stack	O(log n)
Worst recursion stack	O(n)
Stable	No
In-place	Generally yes