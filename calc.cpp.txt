# include <iostream>
using namespace std;

int main() {

  char op;
  float num1, num2;

  cout << "Enter operator: s (square), r (square root), +, -, *, /: ";
  cin >> op;

  cout << "Enter your operand(s): (leave 0 as the second number for square and square root)";
  cin >> num1 >> num2;

  switch(op) {
    
    case 's':
      cout << num1 << " squared " << " = " << num1 * num1;
      break;

   // case 'r':
   //   cout << num1 << " root " << " = " << num1 / num1;
   //   break;

    case '+':
      cout << num1 << " + " << num2 << " = " << num1 + num2;
      break;

    case '-':
      cout << num1 << " - " << num2 << " = " << num1 - num2;
      break;

    case '*':
      cout << num1 << " * " << num2 << " = " << num1 * num2;
      break;

    case '/':
      cout << num1 << " / " << num2 << " = " << num1 / num2;
      break;

    default:
      // If the operator is other than +, -, * or /, error message is shown
      cout << "Error! operator is not correct";
      break;
  }

  return 0;
}
