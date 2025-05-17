# pattern-with-spaces-3-for-loop.c
// C program to print pattern with spaces  ABCDEDCBA  ABCDCBA   ABCBA    ABA     A    
// C program to print pattern with spaces

ABCDEDCBA
 ABCDCBA
  ABCBA
   ABA
    A
    
#include <stdio.h>
int main() { 
    int i,j;
    for(i=0;i<5;i++)
    {
        for(j=0;j<=i-1;j++)
         printf(" ");
        for(j=0;j<=4-i;j++)
         printf("%c",65+j);
        for(j=3-i;j>=0;j--)
         printf("%c",65+j);
        printf("\n");
    }
    return 0;
}
