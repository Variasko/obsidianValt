# While
```cpp
#inclide <iostream>

using namespace std;

int main(){
	
	char isAgain = 'y';
	while (isAgain == 'y')
	{
		cout << "**Игровой процесс**" << endl;
		cout << "Повторим? [y/n]" << endl;
		cin >> isAgain;
	}
	cout << "Ок, пока!" << endl;
	
	return 0;
}
```
