// pyramidprinting.cpp : Defines the entry point for the console application.
//

#include "stdafx.h"
#include<iostream>
#include<conio.h>

using namespace std;
void printpyramid(int integer)
{
	//for top pyramid
	for (int i = 0; i < integer; i++)
	{
		for (int k = i; k <=integer ; k++)
		{
			cout <<"  ";
		}
		for (int j = 0; j <= i; j++)
		{
			cout << "*   ";
		}
		cout << endl;
		
	}
	//for bottom pyramid
	for (int i = 2; i <= integer; i++)
	{
		for (int j = 0; j <= i; j++)
		{
			cout << "  ";
		}
		for (int k = i; k <= integer; k++)
		{
			cout << "*   ";
		}
		cout << endl;
		
	}
}


int main()
{
	//this program developed by anoop
	cout << "this program is to print diamond in * " << endl;
	int input;
	cout << "please enter the number of rows" << endl;
	cin >> input;
	printpyramid(input);
	_getch();
    return 0;
}

