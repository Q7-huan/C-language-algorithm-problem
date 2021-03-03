````C
#include <iostream>
#include <vector>
#include <string.h>
#include <algorithm>//sort()函数头文件
using namespace std;

bool compare(int a, int b) {
	return a > b;
}

int main(void) {
	int a[10] = { 2,4,1,23,5,76,0,43,24,65 }, i;
	for (i = 0; i < 10; i++) {
		cout << a[i] << ",";
	}
	cout << endl;
	sort(a, a + 10, compare);
	for (i = 0; i < 10; i++) {
		cout << a[i] << ",";
	}
	return 0;
}
````

