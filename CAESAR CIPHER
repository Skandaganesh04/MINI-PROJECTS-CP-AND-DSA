#include<stdio.h>
#include<string.h>
#include<stdlib.h>
#include<ctype.h>
#define SIZE 26

void encode(char a[],int b) 
{
    char arr[50];
    int i,val,enval;
    char lowcase,upcase;
        if(a[i]>='A' && a[i]<='Z') 
        {
        upcase='A';
        upcase='Z';
        } 
            else if(a[i]>='a'&& a[i]<='z') 
            {
            lowcase='a';
            lowcase='z';
            } 
                else 
                {
                printf("Invalid Character");
                exit(0);
                }
    for(i=0;i<strlen(a);++i)
    {
        val=a[i];
        enval=val+b;
        if(enval>122) 
        {
            enval=97+(enval-123)%SIZE;
        }
        arr[i]=(char)enval;
    }
    arr[i]='\0';
    printf("The encoded message is %s\n",arr);
}

void decode(char a[], int b) 
{
    char arr[50];
    int i,val,deval;
    for(i=0;i<strlen(a);++i) 
    {
       val=a[i];
       deval=val-b;
       if(deval<97) 
       {
            deval=123-(97-deval)%SIZE;
       }
        arr[i]=(char)deval;
    }
    arr[i]='\0';
    printf("The decoded message is %s\n",arr);
}

int main() 
{
    char str[50],a[10];
    int b;
    printf("Type encode to encrypt and decode to decrypt: ");
    scanf("%s",a);
    printf("\nType the message: ");
    scanf("%s",str);
    printf("\nEnter the number of shifts: ");
    scanf("%d",&b);
    if(strcmp(a,"decode")==0)
        decode(str,b);
    else if(strcmp(a,"encode")==0)
        encode(str,b);
    return 0;
}
