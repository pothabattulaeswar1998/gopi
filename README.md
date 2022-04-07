# gopi
file handling on code


#include <stdio.h>
#include <string.h>
#include <stdlib.h>


int main()
{
        FILE *fp = fopen("eshwar.txt","a");
        char arr[10];

        if(fp == NULL)
        {
                printf("Unable to open file\n");
                return -1;
        }

        memset(arr, '*', sizeof(arr));

        while( fgets( arr, sizeof(arr), fp) != NULL )
        {

                printf("%s\n",arr);
        }


        return 0;

}


