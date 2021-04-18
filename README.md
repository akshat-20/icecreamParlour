# icecreamParlour

### Problem
Cream-chills is a famous chain of ice-cream parlours offering a variety of delicious ice-cream sundaes. The ice-cream sundaes offered here can be customized according to the customer’s demands. The customers can choose the flavour of their ice cream sundae and the toppings that they want to have in their ice-cream sundae from the provided menu. It is fixed that one bowl of sundae will contain two scoops of ice-cream with the desired toppings and then it is served to the customer.

### Solution
For achieving the required output we have used a combination of two design patterns – template method design pattern and decorator method design pattern.

In template pattern, an abstract class ( Icecream ) shows defined ways to execute its methods( templateMethod(), addScoops(), serve(), getPrice(), getName() ). Its subclasses (Strawberry, CaramelApple, Chocolate, Pineapple ) can override the method implementation as per need but the invocation is to be in the same way as defined by an abstract class. As, the ice-cream parlour follows a defined way and follows a fixed procedure so template method pattern is the right choice.

Decorator design pattern is used as this pattern creates a decorator class which wraps the original class (Icecream) and provides additional functionality (adding toppings as per user’s requirement) keeping class methods signature intact. So, here adding toppings (like brownie bites, oreo, caramel, choco-chips, nuts, fruits and sprinkles) is an additional functionality that we have to add to the ice-cream and we have to generate a bill as well.
