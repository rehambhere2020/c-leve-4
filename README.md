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
	#include <string>
	string ReadName() {
		string name;
		getline(cin, name);
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

-check even or odd 
``` c++
	// c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
using namespace std;
#include <string>
enum enumNumber {odd=1 , even =2};
int ReadNum() {
	int num;
	cin >> num;
	return num;
}
enumNumber checkNum(int num) {
	int res = num % 2;
	if(res == 0) {
		return enumNumber::even;
	}
	else {
		return enumNumber::odd;
	}

}

void printNumber(enumNumber num) {
	if (num == enumNumber::even) {
		cout << "Even" << endl;
	}
	else {
		cout << "Odd" << endl;
	}
}

int main()
{
	printNumber(checkNum(ReadNum()));
	return 0;
}


```



