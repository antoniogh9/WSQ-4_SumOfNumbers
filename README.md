# WSQ-4_SumOfNumbers
This program asks the user for a lower and upper value and then prints the sum of the numbers in that range (inclusive). 
/*
SumOfNumbers.cpp
Aug 26, 2017
Dulca
*/
#include <iostream>
using namespace std;
int main() {
	int Lower, Upper, Low,TotalSum ;
	TotalSum = 0 ;

	//User Input Data
		cout << "We will calculate the sum of integers in the range you provide." << endl ;
		cout << "Please give us the lower bound:" << endl ;
		cin >> Lower ;

		cout << "Please give us the upper bound:" << endl ;
		cin >> Upper ;

	//In case the user gives wrong values to Lower and Upper
		while (Lower > Upper) {
			cout << "ERROR" << endl ;
			cout << "Make sure you are giving the lower and upper bound correctly." << endl ;
			cout << "Please give us the lower bound:" << endl ;
			cin >> Lower ;

			cout << "Please give us the upper bound:" << endl ;
			cin >> Upper ;
		}
	Low = Lower ;

	//To calculate the TotalSum
		while (Low <= Upper) {
			TotalSum = TotalSum + Low ;
			Low = Low + 1 ;
		}

	//Output
		cout << "The sum from " << Lower << " to " << Upper << " (inclusive) is: " << TotalSum << endl ;
return 0;
}
