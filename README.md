# stack-


stack operation using array

#include<stdio.h>

#include<stdlib.h>   

void push();

void pop();

void display();

int m,x,i,a[100],top;

int main()

{

int c;

printf("enter the max no. of elements :");

scanf("%d",&m);

while(1)

{

printf("\n 1.push        ");

printf("\n 2.pop   ");

printf("\n 3.display       ");

printf("\n 4.Exit       ");

printf("\n--------------------------------------");

printf("\nEnter your choice:\t");

scanf("%d",&c);

switch(c)

{            case 1:

push();

break;

case 2:

pop();

break;

case 3:

display();

break;

case 4:

exit(0);

break;

default:

printf("\n Wrong Choice:\n");

break;

}

}

return 0;

}

void push()

{

if(top>=m)

{

printf("\n\t over flow");



}

else

{

printf(" Enter a value to be pushed:");

scanf("%d",&x);

top++;

a[top]=x;

}

}

void pop()

{

if(top<=1)

{

printf("\n\t under flow");

}

else

{

printf("\n\t The popped elements is %d",a[top]);

top--;

}

}

void display()

{

if(top>0)

{

printf("\n The elements in STACK \n");

for(i=top; i>0 i--)

printf("\n%d",a[i]);

printf("\n Press Next Choice");

}

else

{
        printf("\n The STACK is empty");

}

}



