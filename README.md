# Đệ quy.Quá trình tính giai thừa 
---------------------
Sử dụng đệ quy viết chương trình thể hiện quá trình tính giai thừa của một số nguyên không âm.

[Input](https://en.wikipedia.org/wiki/Markdown)

> Số nguyên n (0 <= n <= 12)

----
[Output](https://en.wikipedia.org/wiki/Markdown)

>Quá trình tính giai thừa của n. 

Example :

Input:
4

Output:

 0! = 1

 1! = 1

 2! = 2

 3! = 6

 4! = 24

----
## Solution

----
	public int qt_tinhGT(int n) {
		int v;
		if (n == 0) {
			System.out.println(n + "! = " + 1);
			return 1;
		}
		v = n * qt_tinhGT(n - 1);
		System.out.println(n + "! = " + v);
		return v;
	}

