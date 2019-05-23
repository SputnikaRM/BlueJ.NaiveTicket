# NaiveTicket

The second Objects lab, from the BlueJ book's second chapter.

Look for the [Chapter 2 file](./doc/BlueJ-objects-first-ch2.pdf) you need in the [doc](./doc) folder.
There is 35 pages of reading and exercises in the chapter.

Work through all these exercises. You edit this file with your answers for these exercises.

### Exercise 2.1
* Create a TicketMachine object on the object bench.
* Upon viewing its methods, `getBalance`, `getPrice`, `insertMoney`, `printTicket`.
* Use `getPrice` method to view the value of the price of the tickets that was set when this object was created.
* Use `insertMoney` method to simulate inserting an amount of money into the machine.
* Use `getBalance` to check that the machine has a record of the amount inserted.
	* You can insert several separate amounts of money into the machine, just like you might insert multiple coins or notes into a real machine. Try inserting the exact amount required for a ticket. As this is a simple machine, a ticket will not be issued automatically, so once you have inserted enough money, call the `printTicket` method. A facsimile ticket should be printed in the BlueJ terminal window.

### Exercise 2.2
* What value is returned if you check the machine’s balance after it has printed a ticket?
VALUE IS 0.
### Exercise 2.3
* Experiment with inserting different amounts of money before printing tickets.
	* Do you notice anything strange about the machine’s behavior?
	* What happens if you insert too much money into the machine – do you receive any refund?			NO REFUND
	* What happens if you do not insert enough and then try to print a ticket?
	NO REFUND
### Exercise 2.4
* Try to obtain a good understanding of a ticket machine’s behavior by interacting with it on the object bench before we start looking at how the `TicketMachine` class is implemented in the next section.

### Exercise 2.5
* Create another ticket machine for tickets of a different price.
	* Buy a ticket from that machine. 
	* Does the printed ticket look different?  THE PRICE ON THE TICKET IS DIFFERENT

### Exercise 2.6
* Write out what you think the outer wrappers of the `Student` and `LabClass` classes might look like – do not worry about the inner part.

public class Student
public class LabClass

### Exercise 2.7
Does it matter whether we write<br>
`public class TicketMachine`<br>
or<br>
`class public TicketMachine`<br>
in the outer wrapper of a class?   YES

* Edit the source of the `TicketMachine` class to make the change and then close the editor window.
	* Do you notice a change in the class diagram? DOESN'T COMPILE
	* What error message do you get when you now press the compile button? <IDENTIFIER EXPECTED>
	* Do you think this message clearly explains what is wrong? NO

### Exercise 2.8
* Check whether or not it is possible to leave out the word `public` from the outer wrapper of the `TicketMachine` class.

### Exercise 2.9
* From your earlier experimentation with the ticket machine objects within BlueJ you can probably remember the names of some of the methods – `printTicket`, for instance.
	* Look at the class definition in Code 2.1 and use this knowledge, along with the additional information about ordering we have given you, to try to make a list of the names of the fields, constructors, and methods in the `TicketMachine` class.
	* Hint: There is only one constructor in the class.
FIELDS: PRICE BALANCE TOTAL
CONSTRUCTOR: TicketMachine
METHODS: insertMoney, printTicket, getBalance, getPrice


### Exercise 2.10
* Do you notice any features of the constructor that make it significantly different from the other methods of the class? SAME NAME AS THE NAME OF THE CLASS

### Exercise 2.11
* What do you think is the type of each of the following fields?

```java
private int count;	INT
private Student representative; STRING
private Server host;	STRING
```

### Exercise 2.12
* What are the names of the following fields?

```java
private boolean alive; alive
private Person tutor; tutor
private Game game; game
```
### Exercise 2.13

In the following field declaration from the TicketMachine class<br>

```java
private int price;
```
does it matter which order the three words appear in?
* Edit the `TicketMachine` class to try different orderings. After each change, close the editor.
	* Does the appearance of the class diagram after each change give you a clue as to whether or not other orderings are
possible?
	* Check by pressing the compile button to see if there is an error message.
	* Make sure that you reinstantiate the original version after your experiments!

Error occurs. Doesn't compile

### Exercise 2.14
* Is it always necessary to have a semicolon at the end of a field declaration?
* Once again, experiment via the editor.
* The rule you will learn here is an important one, so be sure to remember it.

'; expected error occurs


### Exercise 2.15
* Write in full the declaration for a field of type `int` whose name is `status`.

private int status

### Exercise 2.16
* To what class does the following constructor belong?
```
public Student(String name)

Class : student
```

### Exercise 2.17
* How many parameters does the following constructor have and what are their types?
```
public Book(String title, double price)

2 parameters : string, double
```

### Exercise 2.18
* Can you guess what types some of the `Book` class’s fields might be? String, int, boolean
* Can you assume anything about the names of its fields? Nameofbook, have you read it, serial number, pages, author, 

Work all Exercises from 2.19 to 2.58 that are **NOT** marked *Challenge exercise*.
READ upto and INCLUDING section 2.15 of this chapter.

2.19: name = petsName;
2.21: getPrice: returns the price of the ticket
	getBalance: returns the money left over after printing out the ticket
2.22: getBalance: how much money is returned after the ticket is printed
2.23: The return statement doesn't need to be changed;
2.24: getTotal: the amount of money collected plus the balance
2.25: when you delete the return statement: it says missing return statement
2.26: getPrice method signature: return statement
	printTicket method signature: variable balance and balance being initialized
2.27: insertMoney and printTicket don't have return statements; they both start with public void.
2.29: setPrice is a method because it is a void type
2.30: price = ticketCost;
2.31: score += points;
2.32: price = price - amount;
2.35: ticket prices are different; the input was different so the price is different;
2.36: it would print out the string price instead of the price
2.37: the string # price cents would be the output
2.38: neither of them would should the different prices because they both don't call out the price variable
2.39: it no longer asks for the price of the ticket. 
2.40: mutator because it changes the price;
2.41: this is a mutator method because it changes the state of the object;
2.42: TicketMachine (price);
	TicketMachine() {};
2.45: the boolean is isVisible; yes it was well suited.
2.47
2.49: saving = price * discount
2.50: mean = total / count
2.51: if (price > budget) {
	System.out.println("Just right");
}
2.52: if (price>budget) {
	System.out.println("The price is too high. The budget is " + budget);
}
2.53: the refund balance will always be always be 0;
2.54: doesn't compile because the return statement has to be the last statement
2.56: emptyMachine is an accessor because it tells the current state of the total; it is also a mutator because it changes the value of total.

