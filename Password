#include<stdio.h>
#include<stdlib.h>
#include<time.h>
#include<string.h>
void main()
{
    int letters,num,sym,total,i;
    char password[100];
    char LETTERS[]="ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz";
    char numbers[]="1234567890";
    char symbols[]="!@#$^&*()";


    printf("Welcome to password generator\n");
    printf("\nHow many letters do you want in your password?");
    scanf("%d",&letters);
     printf("\nHow many numbers do you want in your password?");
    scanf("%d",&num);
     printf("\nHow many symbols do you want in your password?");
    scanf("%d",&sym);

    total=letters+num+sym;


    
    
      srand(time(NULL));

      printf("\nThe password as per your requirements is:");

    for(i=0;i<letters;i++)
    {
       printf("%c",LETTERS[rand() % strlen(LETTERS)]);
    }

    for( i=0;i<num;i++)
    {
       printf("%c",numbers[rand() % strlen(numbers)]);
    }

    for( i=0;i<sym;i++)
    {
      printf("%c",symbols[rand() % strlen(symbols)]);
    }

  printf("\n");
}
