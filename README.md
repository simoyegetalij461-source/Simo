#include <iostream>
using namespace std;

int main()
{
    float a, b;
    char op;

    cout << "Enter operator (+, -, *, /): ";
    cin >> op;

    cout << "Enter two numbers: ";
    cin >> a >> b;

    switch (op)
    {
        case '+':
            cout << "Result = " << a + b;
            break;
        case '-':
            cout << "Result = " << a - b;
            break;
        case '*':
            cout << "Result = " << a * b;
            break;
        case '/':
            if (b != 0)
                cout << "Result = " << a / b;
            else
                cout << "Error! Division by zero";
            break;
        default:
            cout << "Invalid operator";
    }

    return 0;
}
