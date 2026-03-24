\## UC1: Display Hello World



\### Description

Print a simple "Hello World" message in the console.



\### Preconditions

Java environment is installed and configured.



\### Main Flow

1\. Program starts

2\. main() method executes

3\. Prints "Hello World"



\### Post Conditions

Message is displayed successfully.



\### Code Example

```java

System.out.println("Hello World");

###########################################################
## UC2: Display User Name

### Description
Accept a name from command-line and display greeting.

### Preconditions
User provides name as argument.

### Main Flow
1. Read args[0]
2. Print greeting

### Post Conditions
Greeting is displayed.

### Concepts Learned
- Command-line arguments
- String concatenation
###########################################################


## UC3: Display Hello with Command-Line Argument or Default

### Description
Displays greeting using a command-line argument if provided.
If no argument is given, defaults to "World".

### Disadvantage of UC2
UC2 crashes when no argument is provided.

### Preconditions
Program may or may not receive input.

### Main Flow
1. Program starts
2. Check if args.length > 0
3. If true → use args[0]
4. Else → use "World"
5. Print greeting

### Post Conditions
Greeting is displayed correctly with or without input.

### Code Example
String name = (args.length > 0) ? args[0] : "World";

### Concepts Learned
- Default values
- Ternary operator
- Defensive programming
- Command-line arguments
##############################################################

## UC4: Display Hello with Multiple Names

### Description
Displays greeting for multiple names passed via command-line.

### Disadvantage of UC3
UC3 supports only one name.

### Preconditions
Program may receive multiple inputs.

### Main Flow
1. Check args length
2. If > 0 → join all names
3. Else → use "World"
4. Print greeting

### Post Conditions
Greeting includes all names.

### Code Example
String names = String.join(", ", args);

### Concepts Learned
- Arrays
- String.join()
- Looping concept
- Multiple input handling
