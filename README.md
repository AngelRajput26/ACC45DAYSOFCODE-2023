#include<iostream>
using namespace std;
void push();
void pop();
void peak();
void display();
int stack[10];
int top=-1;
int main()
{
 int n;
while(1)
{
cout<<"enter the operation number:";
cin>>n;
switch(n)
{
case 1:
push();
break;
case 2:
 pop();
break;
case 3:
 peak();
break;
case 4:
 display();
break;
default:
 cout<<"invalid entry";
break;
}
}
}
void push()
{
if(top==9)
{
cout<<"stack overflow";
}
else
{
int a;
cout<<"enter the value to be inserted: ";
cin>>a;
top++;
stack[top]=a;
}
}
void pop ()
{
if(top==-1)
{
cout<<"stack underflow";
}
else
{
cout<<stack[top];
top--;
}
}
void peak()
{
if(top==-1)
{
cout<<"stack underflow";
}
else
{
cout<<stack[top];
}
}
void display()
{
if(top==-1)
{
cout<<"stack underflow";
}
else
{
for(int i=top;i>=0;i--)
{
cout<<stack[i]<<"\n";
}
cout<<"\n";
}
}