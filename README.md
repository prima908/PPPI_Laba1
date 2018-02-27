#include <iostream>
using namespace std;
int main()
{
	setlocale (LC_ALL, "Russian");
	int N, K;
do
{
		do
		{
		cout << "Введите число N" << endl;
		cin >> N;
		}
		while (N < 0); 	
	double S=0, a = -1, b;
	for (int i=1; i<=N; i++) 
	{
	b=-a;
	a = -a * (1 + i / 10.);
    S = S + a;
	a=b;
		cout << "S = " << S << endl;
	}
	cout << "Результат --> " << S << endl;
cout << endl << "Если хотите ввести другие числа - введите 1, в противном случае - 0." << endl;
cin >> K;
}
while (K!=0);
	system ("pause");
	return 0;
}
