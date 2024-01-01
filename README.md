#include<stdio.h>
void bubblesort(int A[],int n){
    for(int i=1; i<=n-1;i++){
        for(int j=0; j<=n-1-i; j++){
            if(A[j]>A[j+1]){
               int temp=A[j];
               A[j]=A[j+1];
               A[j+1]=temp;
            }
        }
    }


}
void printarr(int A[],int n){
    for(int i=0;i<n;i++){
        printf("%d",A[i]);
    }
    printf("\n");
}



int main(){
    int arr[]={4,7,1,5,2,3,9,8,6,10};
    int n=10;
    printarr(arr,n);
    bubblesort(arr,n);
    printarr(arr,n);
    return 0;

}

# Shorting-Algoritm-bubble-short-
