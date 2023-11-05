# c-leve-4
- print your name  Name
  ```c++
   #include <iostream>
	using namespace std;
	void printName(string name) {
		cout << name;
	}
	int main()
	{
		printName("reham");
		return 0;
	}


 
  ```
- print and read name
  ```c++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	string ReadName() {
		string name;
		cin >> name;
		return name;
	}
	void printName(string name) {
		cout << name;
	}
	int main()
	{
		printName(ReadName());
		return 0;
	}

  ```






