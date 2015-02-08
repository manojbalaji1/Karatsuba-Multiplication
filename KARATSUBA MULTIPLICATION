# Karatsuba-Multiplication
pheew after so much of effort.Please find cases where the program fall short
#include<iostream>
#include<cmath>
#include<cstring>
#include<cstdio>
#include<cstdlib>
using namespace std;
char ch1[100],ch2[100],w[50],x[50],y[50],z[50],ch3[50];
main()
{
 int j,m,n,i,e,f;
 unsigned long long a=0,b=0,c=0,d=0;
 cout<<"Enter the numbers to be multiplied:";
 cin>>ch1;
 cin>>ch2;
 cout<<"ch1="<<ch1<<"\n"<<"ch2="<<ch2<<"\n";
 m=strlen(ch1);
 n=strlen(ch2);
 cout<<m<<" "<<n<<"\n";
 if(m>n)
 {
 	e=m;
	for(i=0;i<(m-n);i++)
		ch3[i]='0';
	ch3[i]='\0';
	cout<<"ch3= "<<ch3<<"\n";
	strcat(ch3,ch2);
	cout<<"ch3= "<<ch3<<"\n";
	strcpy(ch2,ch3);
	cout<<"ch2="<<ch2<<"\n";
}
else if(m<n) 
{	
	e=n;
	for(i=0;i<(n-m);i++)
		ch3[i]='0';
	ch3[i]='\0';
	cout<<"ch3= "<<ch3<<"\n";
	strcat(ch3,ch1);
	cout<<"ch3= "<<ch3<<"\n";
	strcpy(ch1,ch3);
	cout<<"ch1="<<ch1<<"\n";
}
else
{
	e=n;
	cout<<"ch2="<<ch2<<"\n";
}
f=e/2;
cout<<"f="<<f<<"\n";
for(i=0;i<f;i++)
	w[i]=ch1[i];
w[i]='\0';
cout<<"w="<<w<<"\n";
for(;i<e;i++)
	x[i-f]=ch1[i];
x[i]='\0';
cout<<"x="<<x<<"\n";
for(i=0;i<f;i++)
	y[i]=ch2[i];
y[i]='\0';
cout<<"y="<<y<<"\n";
for(;i<e;i++)
	z[i-f]=ch2[i];
z[i]='\0';
cout<<"z="<<z<<"\n";
a=atoll(w);
cout<<"a="<<a<<"\n";
b=atoll(x);
cout<<"b="<<b<<"\n";
c=atoll(y);
cout<<"c="<<c<<"\n";
d=atoll(z);
cout<<"d="<<d<<"\n";
cout<<"Result:"<<a*c*pow(10,e)+(a*d+b*c)*pow(10,f)+b*d<<"\n";
}
