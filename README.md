# Matrix-Multiplication

#include<iostream>
using namespace std;
int main()
{int a[3][3],b[3][3],mul[3][3]={0};
int i,j,k,p;
cout<<"enter elements for matrix A:\n";
for(i=0;i<3;i++)
{for(j=0;j<3;j++)
cin>>a[i][j];
	}
	cout<<"enter elements for matrix B:\n";
for(i=0;i<3;i++)
{for(j=0;j<3;j++)
cin>>b[i][j];
	}
	cout<<" matrix A:\n";
for(i=0;i<3;i++)
{for(j=0;j<3;j++)
{cout<<a[i][j]<<"\t";}
cout<<"\n";}
	cout<<" matrix B:\n";
for(i=0;i<3;i++)
{for(j=0;j<3;j++)
{cout<<b[i][j]<<"\t";}
	cout<<"\n";}
	cout<<" multiplication of matrix A & matrix B:\n";
for(i=0;i<3;i++)
{for(j=0;j<3;j++)
{for(k=0;k<3;k++)
	{p=a[i][k]*b[k][j];
		mul[i][j]=mul[i][j]+p;}
cout<<mul[i][j]<<"\t";}
cout<<"\n";}
return 0;
}
