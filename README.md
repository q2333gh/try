#include<stdio.h>
#define random 50
#define length 20
int bigger(int m ,int n);
int bigger(int m, int n);
int main()
{	
	int i;
	int array1[length];
	int array2[length];
	for (size_t i = 0; i < length; i++)
	{
		array1[i] = rand() % random;
		if (i % 5 == 0) printf("\n");
		printf("%4d",array1[i]);
		array2[i]=lesser(array1[i], array1[i+1]);
	}
	system("pause");
}
int bigger(int m, int n)
{
	return (m>n)?m:n;
}
int lesser(int m, int n)
{
	return (m>n) ? n : m;
}
