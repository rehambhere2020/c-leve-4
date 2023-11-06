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
```
- half number

```c++

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
- check fail or pass
  ```c++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum() {
		int mark;
		cin >> mark;
		return mark;
	}
	enumMark checkItsPassOrNot (int mark) {
		if (mark >= 50) {
			return enumMark::pass;
		}
		else
		{
			return enumMark::fail;
		}
	}
	void printResult(enumMark mark) {
		if (mark == enumMark::pass) {
			cout << "pass";
		}else{
			cout << "fail";
		}
		
	}
	int main()
	{
		printResult(checkItsPassOrNot(ReadNum()));
		return 0;
	}


  ```
- sumNum 3
  ``` c++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum(int &num1, int &num2,int &num3) {
	;
		cin >> num1;
		cin >> num2;
		cin >> num3;
		return num1 , num2 , num3;
	}
	int sumNum(int num1, int num2, int num3) {
		return (num1 + num2 + num3);
	}
	void printResult(int total) {
		cout << total;
	}
	int main()
	{
		int num1, num2, num3;
		ReadNum(num1, num2, num3);
		printResult(sumNum(num1,num2, num3));
		return 0;
	}


  ```

  - calculate Avg
    ``` c++
	    // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum(int &num1, int &num2,int &num3) {
	;
		cin >> num1;
		cin >> num2;
		cin >> num3;
		return num1 , num2 , num3;
	}
	int sumNum(int num1, int num2, int num3) {
		return (num1 + num2 + num3);
	}
	float AvargaeSum(int num1, int num2, int num3) {
		return (float) sumNum(num1, num2, num3) / 3;
	}
	void printResult(float total) {
		cout << total;
	}
	int main()
	{
		int num1, num2, num3;
		ReadNum(num1, num2, num3);
		printResult(AvargaeSum(num1,num2, num3));
		return 0;
	}
	

    ```

    - pass or vail Avg
      ``` c++
		      // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
		//
		
		#include <iostream>
		using namespace std;
		#include <string>
		enum  enumMark {pass=1, fail=0};
		
		int ReadNum(int &num1, int &num2,int &num3) {
		;
			cin >> num1;
			cin >> num2;
			cin >> num3;
			return num1 , num2 , num3;
		}
		int sumNum(int num1, int num2, int num3) {
			return (num1 + num2 + num3);
		}
		float AvargaeSum(int num1, int num2, int num3) {
			return (float) sumNum(num1, num2, num3) / 3;
		}
		
		
		enumMark checkAvg(float avg) {
			if (avg >= 50) {
				return enumMark::pass;
			}
			else {
				return enumMark::fail;
			}
		}
		void printResult(float avg) {
			if (checkAvg(avg) == enumMark::pass) {
				cout << "your pass " << avg << endl;
			}
			else {
				cout << "your Fail";
			}
		}
		
		
		int main()
		{
			int num1, num2, num3;
			ReadNum(num1, num2, num3);
			printResult(AvargaeSum(num1,num2, num3));
			return 0;
		}


      ```
- Max of Tow Number
- ``` c++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum(int &num1, int &num2) {
	;
		cin >> num1;
		cin >> num2;
		return num1, num2;
	}
	
	int checkMAx(int num1, int num2) {
		int max = 0 ;
		if (num1 > num2) {
			max = num1;
		}
		else {
			max = num2;
		}
		
		return max;
	}
	
	
	void printResult(int max) {
		cout << max;
	}
	
	
	int main()
	{
		int num1, num2;
		ReadNum(num1, num2);
		printResult(checkMAx(num1, num2));
		
	}


  ```

  - print max 3 num
  - ```c++
	    // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum(int &num1, int &num2 , int &num3 ) {
	;
		cin >> num1;
		cin >> num2;
		cin >> num3;
		return num1, num2 , num3;
	}
	
	int checkMAx(int num1, int num2 , int num3) {
		int max = 0 ;
		if (num1 > num2) {
			if (num1 > num3) {
				max = num1;
			}else{
				max = num3;
			}
		}
		else {
			if (num2 > num3) {
				max = num2;
			}else{
				max = num3;
			}
	
		}
		
	
		
		return max;
	}
	
	
	void printResult(int max) {
		cout << max;
	}
	
	
	int main()
	{
		int num1, num2 , num3;
		ReadNum(num1, num2 , num3);
		printResult(checkMAx(num1, num2, num3));
		
	}
	

    ```
- swap
- ```c++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum(int &num1, int &num2 ) {
	;
		cin >> num1;
		cin >> num2;
		return num1, num2 ;
	}
	
	void swapNum(int &num1, int &num2) {
		int temp = 0;
		temp = num1;// قيمة num1 تم تخزينها في temp
	
		num1 = num2;// قيمة num2 تم تخزينها في num1
		num2 = temp;//
		
	}
	
	
	void printResult(int num1 , int num2) {
		cout << num1 << num2;
	}
	
	
	int main()
	{
		int num1, num2 ;
		ReadNum(num1, num2);
		swapNum(num1, num2);
		printResult(num1 , num2);
		
	}


  ```

- rectangle REA
- ``` C++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum(int &num1, int &num2 ) {
	;
		cin >> num1;
		cin >> num2;
		return num1, num2 ;
	}
	
	int RectangleSpace(int a, int b) {
		int res = a * b;
		return res;
	}
	
	
	void printResult(int res) {
		cout << res;
	}
	
	
	int main()
	{
		int num1, num2 ;
		ReadNum(num1, num2);
		printResult(RectangleSpace(num1, num2));
		
	}


  ```
- RectangleBySideAndDiagonal
- ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/d3c18075-28ca-47c9-a32c-1359c2a148e3)

- ```c++
	  // c++level4quastion.cpp : This file contains the 'main' function. Program execution begins and ends there.
	//
	
	#include <iostream>
	using namespace std;
	#include <string>
	enum  enumMark {pass=1, fail=0};
	
	int ReadNum(int &num1, int &num2 ) {
	;
		cin >> num1;
		cin >> num2;
		return num1, num2 ;
	}
	
	int RectangleِBySideAndDiagonal(int a, int b) {
		int res = a * sqrt(pow(b,2) - pow(a,2));
		return res;
	}
	
	
	void printResult(int res) {
		cout << res;
	}
	
	
	int main()
	{
		int num1, num2 ;
		ReadNum(num1, num2);
		printResult(RectangleِBySideAndDiagonal(num1, num2));
		
	}
	

  ```

  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/6063ac45-9432-4d56-a514-69a83d006880)

  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/cc865ef9-fe5a-4fb9-84a0-7065a5d228ce)

  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/e8666545-4d82-421b-b235-cf60460503db)

  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/073c2ac8-42fe-4843-a003-a985c0d81e4f)

  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/a243c268-6aae-415e-a6a9-a921c9092106)

  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/41bff366-c6ea-4c6d-bb5c-69e59dca1409)

  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/cce152f1-423d-493f-b7b3-9816a6a8adc9)
  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/f1541cf2-2879-497f-a725-229eb11036df)
  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/2b92338a-8edf-4391-a078-b6ca6a687094)
  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/635f298b-130c-48e7-99d7-42e8643f0281)
  ![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/b689a06a-78ef-4983-996c-220e83720cc8)


![image](https://github.com/rehambhere2020/c-leve-4/assets/86384217/078f542b-d18c-407a-80c2-82e6870835dc)









