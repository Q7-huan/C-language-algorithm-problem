主要是if---else if----else的使用

还可以使用switch语句

题目：

```
一行，四个数字，第一个数表示小明看中的衣服价格，第二和第三个整数分别表示当天的月份、当天的日期、第四个整数表示是否有优惠券（有优惠券用1表示，无优惠券用0表示）。
```

````C++
#include <iostream>
using namespace std;
int main() {
	int month, day;
	float price, pay;
	int n;
	cin >> price >> month >> day>>n;
	if (month == 11 && day == 11) {
		price = price * 0.7;
		if (n == 1) {
			price = price - 50;
			if (price < 0) {
				price = 0;
				printf("%.2f",price);
			}else {
				printf("%.2f", price);
			}
		}
		else {
			printf("%.2f",price);
		}
	}
	else if (month==12&&day==12) {
		price = price * 0.8;
		if (n == 1) {
			price = price - 50;
			if (price < 0) {
				price = 0;
				printf("%.2f", price);
			}else {
				printf("%.2f", price);
			}
		}
		else {
			printf("%.2f", price);
		}

	}
	else {
		printf("%.2f",price);
	}

	return 0;
}
````

