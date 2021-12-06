# submission-2



#include <iostream>
#include <string>
using namespace std;
#include<math.h>
int main()
{
     cout << "PLEASE ENTER YOUR FULL NAME" << endl;
    string yourname;
    getline(cin, yourname);
    int a;
    int factorial = 1;
    cout << "ENTER A NUMBER TO FIND FACTORIAL,TABLE FROM 1 TO 10,AND POWER FROM 5 TO 10  " << endl;
    cin >> a;
    while (cin.fail())
    {
        cout << "PLEASE ENTER A NUMBER: " << endl;
        cin.clear();
        cin.ignore(1000, '\n');
        cin >> a;
    }
    for (int z = a; z > 0; z--)
    {
        factorial = z * factorial;
    }
    cout << "THE FACTORIAL OF "<< a << " IS " << factorial;

    cout << "\nTHE TABLE OF " << a <<" FROM 1 TO 10 IS " << endl;
    for (int table = 0; table <= 10; table++)
    {
       
        cout << a << " x " << table << " = " << a * table << endl;

    }
    cout << "THE FIFTH POWER OF " << a << " IS " << pow(a,5) << endl;
    cout << "THE SIXTH POWER OF "<< a << " IS " << pow(a,6) << endl;
    cout << "THE SEVENTH POWER OF " << a << " IS " << pow(a,7) << endl;
    cout << "THE EIGHT POWER OF " << a << " IS " << pow(a,8) << endl;
    cout << "THE NINTH POWER OF " << a << " IS " << pow(a,9) << endl;
    cout << "THE TENTH POWER OF " << a << " IS " << pow(a,10) << endl;
}
