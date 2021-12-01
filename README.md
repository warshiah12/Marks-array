# Marks-array
#array 5 subject marks average and sum
#include<iostream>
using namespace std;
int main()
{
	int sum=0,marks[5];
	double avg;
	cout << "Enter the marks of 5 subjects " << endl;
	for (int j = 0; j < 5; j++)
	{
		cin >> marks[j];
		while (cin.fail() || marks[j] < 0 || marks[j]>100)
		{
			cout << "Invalid command! Enter a number again" << endl;
			cin.clear();
			cin.ignore();
			cin >> marks[j];
		}
		sum = sum + marks[j];
		avg = sum / 5;
	}
	
	cout << "Sum : " << sum << endl;
	cout << "Average : " << avg << endl;
	return 0;
}
