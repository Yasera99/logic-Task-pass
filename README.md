# logic-Task-pass
Q1




#include<stdio.h> 

#include<conio.h>
 
#include<string.h> 

void removeChar(char * str, char charToRemmove)
{ int i, j; 

int len = strlen(str);
 
for(i=0; i<len; i++)
 
{ if(str[i] == charToRemmove) 
{ for(j=i; j<len; j++)
{ str[j] = str[j+1];
} len--; 
i--;
} } } 
void main()
{ char str[100],ch,c; 

int i,j,len; 
printf("enter the string : \n"); 

scanf("%[^\n]%c",str,&c); 

printf("enter a char you want to remove : "); 
scanf("%c",&ch); 

removeChar(str,ch); 

printf("String after removing '%c': %s", ch, str); 
getch();
 }




Q2


#include <stdio.h> 

#include <stdlib.h>



void main() 

{ 

int num1, num2, i, j, flag, temp, count =0;



printf("Enter the value of num1 and num2 \n"); 

scanf("%d %d", &num1, &num2); 

if (num2 < 2) 

{ 

printf("There are no primes upto %d\n", num2); 

exit(0); 

} 

printf("Prime numbers are \n"); 

temp = num1; 

if ( num1 % 2 == 0) 

{ 

num1++; 

} 

for (i = num1; i <= num2; i = i + 2) 

{ 

flag = 0; 

for (j = 2; j <= i / 2; j++) 

{ 

if ((i % j) == 0) 

{ 

flag = 1; 

break; 

} 

} 

if (flag == 0) 

{ 

printf("%d\n", i); 

count++; 

} 

}
printf("Number of primes between %d & %d = %d\n", temp, num2, count); 

}




Q3


#include <iostream> 

#include <string> 

using namespace std; 

  

// Function that return count of the given 

// character in the string 

int count(string s, char c) 

{ 

    // Count variable 

    int res = 0; 

  

    for (int i=0;i<s.length();i++) 

  

        // checking character in string 

        if (s[i] == c) 

            res++; 

  

    return res; 

} 

  

// Driver code 

int main() 

{ 

    string str= "geeksforgeeks"; 

    char c = 'e'; 

    cout << count(str, c) << endl; 

    return 0; 

}
__





