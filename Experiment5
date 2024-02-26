#include <stdio.h>

#define MAX_SIZE 100

int main() {
    int arr[MAX_SIZE];
    int size, i, choice;

    printf("Enter the size of the array (max %d): ", MAX_SIZE);
    scanf("%d", &size);

    // Input array elements
    printf("Enter %d elements:\n", size);
    for (i = 0; i < size; i++) {
        scanf("%d", &arr[i]);
    }

    // Ask user for operation choice
    printf("Enter 1 for insertion, 2 for deletion at end: ");
    scanf("%d", &choice);

    switch (choice) {
        case 1:
            // Insertion at the end
            if (size >= MAX_SIZE) {
                printf("Array is full, cannot perform insertion.\n");
            } else {
                int element;
                printf("Enter the element to insert: ");
                scanf("%d", &element);

                arr[size] = element; // Insert element at the end
                size++; // Increase array size after insertion

                printf("Element inserted at the end successfully.\n");
            }
            break;
        case 2:
            // Deletion at the end
            if (size == 0) {
                printf("Array is empty, cannot perform deletion.\n");
            } else {
                size--; // Decrease array size to remove the last element

                printf("Element deleted from the end successfully.\n");
            }
            break;
        default:
            printf("Invalid choice.\n");
            break;
    }

    // Print the updated array
    printf("Array after operation:\n");
    for (i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");

    return 0;
}
