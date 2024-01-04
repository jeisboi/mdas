#include <iostream>
using namespace std;

int main() {
    while (true) {
        int numOne, numTwo;
        char mdasOpe;

        cout << "\t\tAdd (1) Subtract (2) Multiply (3) Divide (4) ";
        cout << "\t\tEnter Choice: ";
        cin >> mdasOpe;

        switch (mdasOpe) {
        case '1':
            cout << "input first value to calculate" << endl;
            cin >> numOne;

            cout << "input second value to calculate" << endl;
            cin >> numTwo;

            cout << numOne << " + " << numTwo << " = " << numOne + numTwo << endl;

            break;
        case '2':
            cout << "input first value to calculate" << endl;
            cin >> numOne;

            cout << "input second value to calculate" << endl;
            cin >> numTwo;

            cout << numOne << " - " << numTwo << " = " << numOne - numTwo << endl;

            break;

        case '3':
            cout << "input first value to calculate" << endl;
            cin >> numOne;

            cout << "input second value to calculate" << endl;
            cin >> numTwo;

            cout << numOne << " * " << numTwo << " = " << numOne * numTwo << endl;

            break;
        case '4':
            cout << "input first value to calculate" << endl;
            cin >> numOne;

            cout << "input second value to calculate" << endl;
            cin >> numTwo;

            cout << numOne << " / " << numTwo << " = " << numOne / numTwo << endl;

            break;

        default:
            cout << "Invalid choice. Please try again." << endl;
            continue;  
        }

        cout << "Do you want to perform another calculation? (y/n): ";
        char repeatChoice;
        cin >> repeatChoice;

        if (repeatChoice != 'y' && repeatChoice != 'Y') {
            break;  
        }
        system("cls");

    }

    return 0;
}
