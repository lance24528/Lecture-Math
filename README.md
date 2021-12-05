#include <iostream>
#include <string>
#include <iomanip>
#include <array>
#include <math.h>


using namespace std;

int main()
{
	double number;	
	cout << "Input a number \n";

	cin >>  number;
	while (cin.fail())
	{
		cin.clear();
		cin.ignore();
		cout << "\nInvalid Input try again \n\nInput a number \n\n";
		cin >> number;
	}
	cout << "square root: " << sqrt(number) << " cube root: " << cbrt(number);

}
