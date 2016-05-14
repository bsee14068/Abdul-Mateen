# Abdul-Mateen
 include <iostream>
#include <cstdio>
#include <cstdlib>
#include <conio.h>
#include <cstring>
#include <string>

using namespace std;
class Accounts{
	private:
		//string name;
		int acc_num; 
		//string addr;
		//int cnic;
		int bal;
		int pin;
	public:
		Accounts()
		{

		}

		Accounts(int ac,int ba,int pi);

	//~Accounts();
	void setAccNum(int num)
		{
			this->acc_num = num;

		}
		int getAccInfo()

		{

			return this->acc_num;

		}
};
Accounts::Accounts(int ac,int ba,int pi)

{

	//name="abc";

	acc_num=ac;

	//addr="xyz";

	//cnic=0123456789123;

	bal=ba;

	pin=pi;

}

/*

Accounts::~Accounts()

{

	

	//delete name;

	//delete addr;

	//delete cnic;

}

*/




class ATM{

	int* AccInfo;

		public:

			ATM()

			{

				AccInfo = new int [0001, 0002, 0003];

			}

						

		void withdraw();

		void transaction();

		int check_bal();

		void pay_bill();

		int pin_check(int);
		int account_check(Accounts&);
};
int ATM::account_check(Accounts& a)
{
	/*
	for (int i=0;i<3;i++)
	{
		if (acc=a[i].acc_num)
	}
	*/
}
int main (void)
{
	Accounts a[3];
	a[0].setAccNum(0001);
	//a[1].Accounts(0002,2000,1122);
	//a[2].Accounts(0003,5000,1133);
	
	int acc;

	cout << "Please enter your account number :\n";

	cin >> acc;

	cout << a[0].getAccInfo();
}
