# Exception-Handling-in-CPP
C++ exception handling is built upon three keywords: try, catch, and throw. throw − A program throws an exception when a problem shows up. catch − A program catches an exception with an exception handler at the place in a program where you want to handle the problem.


//1.To throw exception when j=1
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#include<iostream>
uing namespace std;

int main()
{
  int x,y;
  cout<<"\n Enter the values of X & Y";
  cin>>x>>y;
  int j;
  j=x>y?0:1:
  
  try
  {
    if(j==0)
    {
       cout<<"\n Substraction (x-y)="<<x-y<<"\n";
    }
    else
    {  throw(j);  }
  }
  
  catch(int k)
  {
     cout<<"Exception caught:j="<<j<<"\n";
  }
  return 0;
  }
  
  ===================
  
  
  
//2.To define function that generates exception
  ~~~~~~~~~~~~~~~~~~~~~~
  #include<iostream>
  void sqr()
  {
    int s;
    cout<<"\n Enter the number";
    cin>>s;
    if(s>0)
    {
       cout<<"\n Square="<<s*s;
    }
    else
    {
    throw(s); 
    }
  }
  
  int main()
  {
   try
   {
    sqr();
    sqr();
   }
   
   catch(int j)
   {
    cout<<"\n Caught the exception \n";
   }
   
   return 0;
   }
   
   ================================
   
   //3.Throw multiple exceptions
   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   
   #include<iostream>
   using namespace std;
   
   void num(int k)
   {
     try{
     if(k==0)
     {
       throw k;
     }
     else if(k>0) 
     {
       throw p;
     }
     else if(k<0)
     {
       throw O;
     }
     cout<<"\n *********try Block***********"<<endl;
    }
 
 
   
