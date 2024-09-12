# COP-2334-1-Pizza-Delivery-Programming-Assignment
This is a repository link of the Module 3 Assignment for COP 2334-1

// This assignment is created by Carlos Gonzalez
// A calculation of a pizza delivery order.
#include <iostream>
#include <iomanip>
using namespace std;

// Main function
int main() {

  // Declare variables
  cout << fixed << setprecision(2);

  // This variable declares the numebr of pizzas ordered
  int numberOfPizzas;
  // This variable declares the cost per pizza
  const double costPerPizza = 14.99;
  // This variable declares the tax rate
  const int salesTax = 8;
  // This variable declares the initial price of the pizza
  double pizza_Subtotal = 0;
  // This variable declares the total cost of the order
  double pizza_Total = 0;

  // This line of code asks the user to input the number of pizzas they would like to order
  cout << "How many pizzas would you like to order? ";
  cin >> numberOfPizzas;
  // These statements calculates the subtotal of the order
  pizza_Subtotal = numberOfPizzas * costPerPizza;
  // These statements calculates the total cost of the order
  pizza_Total = pizza_Subtotal + (pizza_Subtotal * salesTax / 100);
  // These statements display the subtotal and total cost of the order
  cout << "Subtotal: $" << pizza_Subtotal << endl;
  cout << "Total: $" << pizza_Total << endl;
  return 0;
}
