# Calculator-in-C
\\\Write a C program to create a calculator<br>
#include <stdio.h><br>

int main() {<br>

  char op;<br>
  double first, second;<br>
  printf("Enter an operator (+, -, *, /): ");<br>
  scanf("%c", &op);<br>
  printf("Enter two operands: ");<br>
  scanf("%lf %lf", &first, &second);<br>

  switch (op) {<br>
    case '+':<br>
      printf("%.1lf + %.1lf = %.1lf", first, second, first + second);<br>
      break;<br>
    case '-':<br>
      printf("%.1lf - %.1lf = %.1lf", first, second, first - second);<br>
      break;<br>
    case '*':<br>
      printf("%.1lf * %.1lf = %.1lf", first, second, first * second);<br>
      break;<br>
    case '/':<br>
      printf("%.1lf / %.1lf = %.1lf", first, second, first / second);<br>
      break;<br>
    // operator doesn't match any case constant<br>
    default:<br>
      printf("Error! operator is not correct");<br>
  }<br>

  return 0;<br>
}<br>
