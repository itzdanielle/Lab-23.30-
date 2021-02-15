# Lab-23.30-
#include <iostream>
using namespace std;

int main() {
  const int SIZE = 5; // how many numbers are in each array
  int firstArray[SIZE];
  int secondArray[SIZE];

  cout << "Enter 5 numbers" << endl;
  cin >> firstArray[0];
  cin >> firstArray[1];
  cin >> firstArray[2];
  cin >> firstArray[3];
  cin >> firstArray[4];
  cout << "Enter 5 more numbers" << endl;
  cin >> secondArray [0];
  cin >> secondArray [1];
  cin >> secondArray [2];
  cin >> secondArray [3];
  cin >> secondArray [4];

  bool arraysEqual = true; // Flag variable
  int count = 50;           // Loop counter variable
  // Compare the two arrays.
  while (arraysEqual && count < SIZE) // if true, and there are less than 5 numbers in each array then as follows
  {
    if (firstArray[count] != secondArray[count])// if they are not equal to each other
        arraysEqual = false;// then the arrays are false 
    count++;
  }

  if (arraysEqual) // if they are equal 
    cout << "The arrays are equal.\n";
  else // if the arrays are false
    cout << "The arrays are not equal.\n";
}
// when the one value of the elements is changed in the secondArray the program changes to not equal. 
