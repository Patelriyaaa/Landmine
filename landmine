#include <Windows.h>
#include <iostream>
#include <string>
using namespace std;
void main()
{
	int const MAXROWS = 10;
	int const MAXCOLS = 10;
	int r;
	int c;
	int board[MAXROWS][MAXCOLS] =
	{
		//adding the array
		{ 0,0,1,0,0,0,1,0,0,0 },
		{ 0,0,0,0,0,0,0,0,1,0 },
		{ 0,0,1,0,1,0,0,0,0,0 },
		{ 0,0,0,0,0,0,0,0,0,0 },
		{ 0,0,0,0,1,0,0,1,0,0 },
		{ 0,0,0,1,0,0,1,0,0,0 },
		{ 0,1,0,0,0,0,0,0,0,0 },
		{ 0,0,0,0,1,0,0,0,0,1 },
		{ 0,0,0,0,0,0,0,0,1,0 },
		{ 0,0,1,0,0,0,1,0,0,1 }
	};
	while (1)
	{
		// display array.
		system("cls");

		for (int row = 0; row < MAXROWS; row++)
		{
			for (int col = 0; col < MAXCOLS; col++)
				
			{
				if (board[row][col] == 0 || board[row][col] == 1)
				{
					SetConsoleTextAttribute(GetStdHandle(STD_OUTPUT_HANDLE), 15);
					cout << char(219) << " ";
				}
				else if (board[row][col] == 3)cout << "*" << " ";
			}
			cout << endl << endl;
		}
		cout << "Enter r and c" << endl;
		cin >> r >> c;
		if (board[r][c] == 0)
		{
			board[r][c] = 3;
			cout << "safe area" << endl;
		}
		else if (board[r][c] == 1) {
			board[r][c] = 100;
			break;
			// breaks from loop, when it hits bomb
		}
	}
	system("cls");
	{
		// display array.
		system("cls");
		for (int row = 0; row < MAXROWS; row++)
			//prints landmine
		{
			for (int col = 0; col < MAXCOLS; col++)
			{
				if (board[row][col] == 0) //the spaces
				{
					SetConsoleTextAttribute(GetStdHandle(STD_OUTPUT_HANDLE), 25);
					cout << char(219) << " ";
				}
				else if ((board[row][col] == 100))
					// bomb hit
				{
					SetConsoleTextAttribute(GetStdHandle(STD_OUTPUT_HANDLE), 135);
					cout << "U" << char(219);
				}
				else if (board[row][col] == 1)
				{
					SetConsoleTextAttribute(GetStdHandle(STD_OUTPUT_HANDLE), 135);
					cout << " " << char(219);
				}
				else if (board[row][col] == 3)
					//all the safe spaces hit
					cout << "* ";
			}
			cout << endl << endl;
		}
		SetConsoleTextAttribute(GetStdHandle(STD_OUTPUT_HANDLE), 15);
		cout << "  ___  ___  __  __ ___ ___ ___  _ " << endl;
		cout << " | _ )/ _ \|  \/  | _ ) __|   \| |" << endl;
		cout << " | _ \ (_) | |\/| | _ \ _|| |) |_|" << endl;
		cout << " |___/\___/|_|  |_|___/___|___/(_)" << endl;
		
		cout << "          _______             _        _______  _______ _________ _ " << endl;
		cout << "|\     /|(  ___  )|\     /|  ( \      (  ___  )(  ____ \\__   __/( )" << endl;
		cout << "( \   / )| (   ) || )   ( |  | (      | (   ) || (    \/   ) (   | |" << endl;
		cout << " \ (_) / | |   | || |   | |  | |      | |   | || (_____    | |   | |" << endl;
		cout << "  \   /  | |   | || |   | |  | |      | |   | |(_____  )   | |   | |" << endl;
		cout << "   ) (   | |   | || |   | |  | |      | |   | |      ) |   | |   | |" << endl;
		cout << "   | |   | (___) || (___) |  | (____/\| (___) |/\____) |   | |      " << endl;
		cout << "   \_/   (_______)(_______)  (_______/(_______)\_______)   )_(   (_)" << endl;
		cout << "                                                                    " << endl;
system("pause");
	}
}
