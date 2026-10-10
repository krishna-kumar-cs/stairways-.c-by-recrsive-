# stairways-.c-by-recrsive-
find path n stairs if we have three step permission. 
#include<stdio.h>
#include<stdlib.h>
int recway(int n){
    if(n<=3)return n;
    int a = recway(n-1)+recway(n-2)+recway(n-3);
    return a;
}
int main()
{
    int stairs,way;
    printf("enter stairs\n");
    scanf("%d",&stairs);
    way= recway(stairs);
    printf("the total ways are: %d",way);
    return 0;
}