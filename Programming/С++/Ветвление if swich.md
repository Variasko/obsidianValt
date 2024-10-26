# If
```cpp
#inclide <iostream>

using namespace std;

int main(){
	int a = 10;
	bool b = true;
	string c = "a";
	char d = '';

	if (a)
	{
		cout << "А не 0" << endl; //✔
	}
	if (b)
	{
		cout << "B не false" << endl;//✔
	}
	if (c)
	{
		cout << "C не пустота" << endl;//✔
	}
	if (d)
	{
		cout << "D не null" << endl;//🔴
	}
	return 0;
}
```

# Пояснения
If Работает таким образом, что если мы указываем не лог. выражение, а переменную, то в случае, если она не нулевая, будет выполнен блок кода if

# Switch
```cpp
#inclide <iostream>

using namespace std;

int main(){
	int a;
	cin >> a;

	switch (a)
	{
		case 1:
			cout << "1" << endl;
			break;
		case 2:
			cout << "2" << endl;
			break;
		default:
			cout << "Incorrect" << endl;
	}
	return 0;
}
```
