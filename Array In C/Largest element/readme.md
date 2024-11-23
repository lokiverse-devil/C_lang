#Array Code for Finding the largest element in an array in c
#include<stdio.h>
int main()
{
    int arr[5];
    int i, max;
    
    // Input the elements of the array
    for(i = 0; i < 5; i++) {
        printf("Enter the value of %d element: ", i + 1);
        scanf("%d", &arr[i]);
    }
    
    // Initialize max to the first element in the array
    max = arr[0];
    
    // Find the largest element in the array
    for(i = 1; i < 5; i++) { 
        if(arr[i] > max) {
            max = arr[i];
        }
    }
    
    // Output the largest element
    printf("The biggest element in the array is %d\n", max);
    
    return 0;
}
