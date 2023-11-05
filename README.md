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
- ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/5c07fe02-fef8-42f6-bbd9-06edcfb5e423)
  ``` c++
	  	// c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	struct stInfo
	{
		int Age;
		bool HasDrivingLicenes;
	};
	stInfo ReadInfo() {
		stInfo Info;
		cin >> Info.Age;
		cout << "olease enter licens" << endl;
		cin >> Info.HasDrivingLicenes;
		return Info;
	}
	bool isAccepted(stInfo info) {
		return (info.Age > 21 && info.HasDrivingLicenes);
	}
	void printResult(stInfo info) {
		if (isAccepted(info)) {
			cout << "success";
		}
		else {
			cout << "Not Ecepted";
		}
	}
	int main()
	{
		printResult(ReadInfo());
		return 0;
	}


  ```

- has Recomminadation
  ``` c++
	// c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	struct stInfo
	{
		int Age;
		bool HasDrivingLicenes;
		bool HasRecommendation;
	};
	stInfo ReadInfo() {
		stInfo Info;
		cin >> Info.Age;
		cout << "olease enter licens" << endl;
		cin >> Info.HasDrivingLicenes;
		cin >> Info.HasRecommendation;
		return Info;
	}
	bool isAccepted(stInfo info) {
		return (info.HasRecommendation || info.Age > 21 && info.HasDrivingLicenes);
	}
	void printResult(stInfo info) {
		if (isAccepted(info)) {
			cout << "success";
		}
		else {
			cout << "Not Ecepted";
		}
	}
	int main()
	{
		printResult(ReadInfo());
		return 0;
	}
	

  ```
  - Print FullNAm e
    ``` c++
	    	// c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	struct stInfo
	{
		string firstName;
		string LastName;
	};
	stInfo ReadInfo() {
		stInfo Info;
		cin >> Info.firstName;
		cout << "olease enter last name" << endl;
		cin >> Info.LastName;
		return Info;
	}
	string GetFullName(stInfo Info) {
		string fullName = "";
		fullName = Info.firstName + " " + Info.LastName;
		return fullName;
	}
	void printResult(string name) {
		cout << name<<endl;
	}
	int main()
	{
		printResult(GetFullName(ReadInfo()));
		return 0;
	}
	

    ```

- if i want reversed
  ``` c++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	struct stInfo
	{
		string firstName;
		string LastName;
	};
	stInfo ReadInfo() {
		stInfo Info;
		cin >> Info.firstName;
		cout << "olease enter last name" << endl;
		cin >> Info.LastName;
		return Info;
	}
	string GetFullName(stInfo Info,bool reversed) {
		string fullName = "";
		if (reversed) {
			fullName =  Info.LastName + " " + Info.firstName ;
	
		}
		else {
			fullName = Info.firstName + " " + Info.LastName;
	
		}
		return fullName;
	}
	void printResult(string name) {
		cout << name<<endl;
	}
	int main()
	{
		printResult(GetFullName(ReadInfo(),1));
		return 0;
	}
```
### half number 
```
```c++
// c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
using namespace std;
#include <string>
int ReadNum() {
	int num;
	cin >> num;
	return num;
}
float halfNum(int num) {
	if (num == 0) return num;

	return (float)num / 2;
}
void printResult(int  num) {
	cout << halfNum(num);
}
int main()
{
	printResult(ReadNum());
	return 0;
}
```
```
