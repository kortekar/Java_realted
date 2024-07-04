
# Java Cheat Sheet

## Data Types

### Primitive Data Types:
- `int `   :   4 bytes, stores whole numbers from -2,147,483,648 to 2,147,483,647.
- `byte`   :   1 byte, stores whole numbers from -128 to 127.
- `short`  :   2 bytes, stores whole numbers from -32,768 to 32,767.
- `long`   :   8 bytes, stores whole numbers from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807.
- `float`  :   4 bytes, stores fractional numbers, sufficient for storing 6 to 7 decimal digits.
- `double` :   8 bytes, stores fractional numbers, sufficient for storing 15 decimal digits.
- `boolean`:   1 bit, stores true or false.
- `char`   :   2 bytes, stores a single 16-bit Unicode character.

### Reference Data Types:
- `Arrays`
- `Classes`
- `Interfaces`
- `Strings`

## Operators and Precedence

### Arithmetic Operators:
- `+` (Addition)
- `-` (Subtraction)
- `*` (Multiplication)
- `/` (Division)
- `%` (Modulus)

### Relational Operators:
- `==` (Equal to)
- `!=` (Not equal to)
- `>` (Greater than)
- `<` (Less than)
- `>=` (Greater than or equal to)
- `<=` (Less than or equal to)

### Logical Operators:
- `&&` (Logical AND)
- `||` (Logical OR)
- `!` (Logical NOT)

### Bitwise Operators:
- `&` (Bitwise AND)
- `|` (Bitwise OR)
- `^` (Bitwise XOR)
- `~` (Bitwise NOT)
- `<<` (Left shift)
- `>>` (Right shift)
- `>>>` (Unsigned right shift)

### Assignment Operators:
- `=` (Assignment)
- `+=` (Add and assign)
- `-=` (Subtract and assign)
- `*=` (Multiply and assign)
- `/=` (Divide and assign)
- `%=` (Modulus and assign)

### Operator Precedence:
Highest to lowest: `()`, `[]`, `.`, `++/--`, `* / %`, `+ / -`, `<< / >> / >>>`, `< / <= / > / >=`, `== / !=`, `&`, `^`, `|`, `&&`, `||`, `? :`, `=`, `+=`, `-=`, ...


## Control Flow:

### If-Else Statement:
```java
if (condition) {
    // Code block
} else if (anotherCondition) {
    // Code block
} else {
    // Code block
}
```

### Switch Statement:

```java
switch (variable) {
    case value1:
        // Code block for value1
        break;
    case value2:
        // Code block for value2
        break;
    default:
        // Code block if no case matches
}
```

### Types of For Loops in Java:

#### Standard For Loop:
```java
for (int i = 0; i < 5; i++) {
    // Loop body
}
```

#### Enhanced For Loop (for-each loop):
```java
int[] numbers = {1, 2, 3, 4, 5};
for (int number : numbers) {
    // Loop body
}
```
#### For Loop with Iterator (used with collections):
```java
List<String> fruits = Arrays.asList("Apple", "Banana", "Orange");
for (Iterator<String> iterator = fruits.iterator(); iterator.hasNext(); ) {
    String fruit = iterator.next();
    // Loop body
}
```
#### For Loop with Iterable (Java 8 and later):
```java
List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5);
numbers.forEach(number -> {
    // Loop body
});
```
#### While Loop:
```java
int i = 0;
while (i < 5) {
    // Loop body
    i++;
}
```

## Data Structures


### Arrays:

- `[int[] nums] = {1, 2, 3};`
- `nums.length;` // Get length
- `nums[0];` // Access element


### ArrayList:

- `import java.util.ArrayList;`
- `ArrayList<Integer> list = new ArrayList<>();`
- `list.add(1);` // Add element
- `list.get(0);` // Access element
- `list.size();` // Get size
- `list.remove(0);` // Remove element
- `list.clear();` // Clear list


### HashMap:
- `import java.util.HashMap;` // package
- `HashMap<String, Integer> map = new HashMap<>();`
- `map.put("key", 1);` // Insert key-value pair
- `map.get("key");` // Access value by key
- `map.remove("key");` // Remove key-value pair
- `map.size();` // Get size
- `map.containsKey("key");` // Check if key exists
- `map.clear();` // Clear map

### HashSet:

- `import java.util.HashSet;` // package
- `HashSet<Integer> set = new HashSet<>();`
- `set.add(1);` // Add element
- `set.contains(1);` // Check if element exists
- `set.remove(1);` // Remove element
- `set.size();` // Get size
- `set.clear();` // Clear set


## Important Data Structures for Coding Interviews

### Linked List:

```java
class Node {
    int data;
    Node next;
    Node(int data) {
        this.data = data;
        this.next = null;
    }
}
```

### Stack:

- `import java.util.Stack;`
- `Stack<Integer> stack = new Stack<>();`
- `stack.push(1);` // Push element
- `stack.pop();` // Pop element
- `stack.peek();` // Get top element
- `stack.isEmpty();` // Check if stack is empty

### Queue:

- `import java.util.LinkedList;`
- `import java.util.Queue;`
- `Queue<Integer> queue = new LinkedList<>();`
- `queue.add(1);` // Add element
- `queue.poll();` // Remove and return head element
- `queue.peek();` // Get head element
- `queue.isEmpty();` // Check if queue is empty


### Priority Queue:

- `import java.util.PriorityQueue;`
- `PriorityQueue<Integer> pq = new PriorityQueue<>();`
- `pq.add(1);` // Add element
- `pq.poll();` // Remove and return the smallest element
- `pq.peek();` // Get the smallest element
- `pq.isEmpty();` // Check if priority queue is empty


#  Miscellaneous
### Input/Output:

- `import java.util.Scanner;`
- `Scanner scanner = new Scanner(System.in);`
- `int x = scanner.nextInt();` // Read integer input
- `String s = scanner.nextLine();` // Read string input


### Math Functions:

- `import java.lang.Math;`
- `Math.pow(2, 3);` // 2 raised to the power 3
- `Math.sqrt(16);` // Square root of 16
- `Math.max(1, 2);` // Maximum of 1 and 2
- `Math.min(1, 2);` // Minimum of 1 and 2

### String Methods:

- `String str = "hello";`
- `str.length();` // Get length
- `str.charAt(0);` // Get character at index 0
- `str.substring(1, 3);` // Get substring from index 1 to 3
- `str.toUpperCase();` // Convert to uppercase
- `str.toLowerCase();` // Convert to lowercase
- `str.equals("hello");` // Check equality



### Clean Code Tips

1.  **Docstrings and Comments:**
    
    ```
    /**
     * Function to double the value.
     * @param num The number to double.
     * @return The doubled value.
     */
    public int double(int num) {
        return 2 * num;
    }
    
    ```
    
2.  **Assertions:**
    
    ```
    assert x == y : "x and y should be equal";
    
    ```
    
3.  **Modularity:**
    
    -   Break down your code into small, reusable functions.
    -   Avoid code duplication by using methods and classes.


## FEW DIFFERENCE 

#


| Feature      | Array                                             | List                                               | ArrayList                                           |
|--------------|---------------------------------------------------|----------------------------------------------------|-----------------------------------------------------|
| Definition   | Fixed-size data structure                          | Interface representing an ordered collection       | Implementation of List using resizable array         |
| Size         | Fixed                                             | Dynamically resizable                              | Dynamically resizable                               |
| Access       | Index-based (zero-based)                           | Index-based                                       | Index-based                                         |
| Type         | Primitive types or objects                        | Any object type                                   | Any object type                                     |
| Mutability   | Fixed size, cannot be changed                     | Mutable, size can change                          | Mutable, size can change                            |
| Example      | `int[] numbers = new int[5];`                      | `List<Integer> numberList = new ArrayList<>();`   | `ArrayList<String> names = new ArrayList<>();`      |
| Add Element  | Not applicable, fixed size                        | `numberList.add(10);`                             | `names.add("Alice");`                               |
| Delete Element | Not applicable, fixed size                       | `numberList.remove(0);`                           | `names.remove("Alice");`                            |
| Access Element | `int value = numbers[0];`                         | `int firstElement = numberList.get(0);`           | `String firstName = names.get(0);`                  |
| Iterate      | Use `for` loop                                    | Use `for-each` loop or `Iterator`                 | Use `for-each` loop or `forEach` method             |
| Size         | `int size = numbers.length;`                      | `int size = numberList.size();`                   | `int size = names.size();`                          |

#

##    HASHMAP      (vs)      HASHSET 

| Feature        | HashMap                                                      | HashSet                                                      |
|----------------|--------------------------------------------------------------|--------------------------------------------------------------|
| Definition     | Implements `Map` interface, stores key-value pairs           | Implements `Set` interface, stores unique elements           |
| Duplicate Keys | Does not allow duplicate keys                                 | Does not allow duplicate elements                            |
| Null Values    | Allows a single null key and multiple null values            | Allows a single null value                                   |
| Ordering       | Does not guarantee order of elements                         | Does not guarantee order of elements                         |
| Example        | `HashMap<String, Integer> map = new HashMap<>();`             | `HashSet<String> set = new HashSet<>();`                     |
| Add Element    | `map.put("key", 1);`                                          | `set.add("element");`                                        |
| Remove Element | `map.remove("key");`                                          | `set.remove("element");`                                     |
| Check Existence| `boolean exists = map.containsKey("key");`                     | `boolean exists = set.contains("element");`                  |
| Iterate        | `for (String key : map.keySet()) { /* Loop body */ }`         | `for (String element : set) { /* Loop body */ }`             |
| Size           | `int size = map.size();`                                      | `int size = set.size();`                                     |


#

## TreeMap vs TreeSet vs LinkedList

| Feature         | TreeMap                                        | TreeSet                                      | LinkedList                                  |
|-----------------|------------------------------------------------|----------------------------------------------|---------------------------------------------|
| Definition      | Implements `NavigableMap`, stores key-value pairs sorted by keys | Implements `NavigableSet`, stores unique elements sorted by natural order | Doubly-linked list implementation of `List` interface |
| Ordering        | Elements are sorted based on natural order of keys | Elements are sorted based on natural order of elements | Maintains insertion order                     |
| Duplicate Values| Does not allow duplicate keys                    | Does not allow duplicate elements             | Allows duplicate elements                   |
| Null Values     | Does not allow null keys or values               | Does not allow null elements                 | Allows null elements                        |
| Example         | `TreeMap<Integer, String> map = new TreeMap<>();` | `TreeSet<String> set = new TreeSet<>();`     | `LinkedList<String> list = new LinkedList<>();` |
| Add Element     | `map.put(1, "value");`                          | `set.add("element");`                        | `list.add("value");`                        |
| Remove Element  | `map.remove(1);`                                | `set.remove("element");`                     | `list.remove("value");`                     |
| Access Element  | `String value = map.get(1);`                    | Not directly; use `Iterator` or `forEach`    | `String value = list.get(0);`               |
| Iterate         | `for (Integer key : map.keySet()) { /* Loop body */ }` | `for (String element : set) { /* Loop body */ }` | `for (String element : list) { /* Loop body */ }` |
| Size            | `int size = map.size();`                        | `int size = set.size();`                     | `int size = list.size();`                   |

#

## ArrayDeque vs LinkedList

| Feature         | ArrayDeque                                     | LinkedList                                   |
|-----------------|------------------------------------------------|----------------------------------------------|
| Definition      | Implements `Deque`, resizable array-based implementation | Doubly-linked list implementation of `List` interface |
| Access          | Random access O(1) for indexed operations      | Sequential access O(n) for indexed operations |
| Memory Efficiency | More memory efficient for large collections    | Uses more memory due to node overhead        |
| Example         | `ArrayDeque<String> deque = new ArrayDeque<>();` | `LinkedList<String> list = new LinkedList<>();` |
| Add Element     | `deque.add("element");`                        | `list.add("element");`                       |
| Remove Element  | `deque.removeFirst();`                         | `list.removeFirst();`                        |
| Access Element  | `String first = deque.getFirst();`              | `String first = list.getFirst();`            |
| Iterate         | `for (String element : deque) { /* Loop body */ }` | `for (String element : list) { /* Loop body */ }` |
| Size            | `int size = deque.size();`                     | `int size = list.size();`                    |


#

## PriorityQueue vs HashSet
| Feature         | PriorityQueue                                 | HashSet                                       |
|-----------------|------------------------------------------------|-----------------------------------------------|
| Definition      | Implements `Queue`, orders elements based on priority | Implements `Set`, stores unique elements      |
| Ordering        | Orders elements based on priority (natural order or custom comparator) | Does not guarantee any specific order         |
| Example         | `PriorityQueue<Integer> pq = new PriorityQueue<>();` | `HashSet<String> set = new HashSet<>();`       |
| Add Element     | `pq.add(5);`                                   | `set.add("element");`                         |
| Remove Element  | `pq.poll();`                                   | `set.remove("element");`                      |
| Access Element  | `int head = pq.peek();`                        | Not directly; use `Iterator` or `forEach`     |
| Iterate         | `while (!pq.isEmpty()) { /* Loop body */ }`    | `for (String element : set) { /* Loop body */ }` |
| Size            | `int size = pq.size();`                        | `int size = set.size();`                      |




### Technical Topics to Review:
1. `Data Structures and Algorithms`: Focus on common data structures (arrays, linked lists, trees, graphs, hash tables) and algorithms (sorting, searching, dynamic programming).
   
2. `Object-Oriented Programming (OOP)`: Understand concepts like inheritance, polymorphism, encapsulation, and abstraction.

3. `Java Core Concepts`: Including exception handling, multithreading, generics, collections framework (ArrayList, HashMap, etc.), and Java I/O.

4. `Database Basics`: SQL queries, relational database concepts (joins, normalization), and JDBC for Java database connectivity.

5. `Web Technologies`: HTTP protocol, RESTful APIs, servlets, JSP, Spring framework basics, and MVC architecture.

6. `Testing`: Unit testing with JUnit or TestNG, mocking frameworks like Mockito, and integration testing.

7. `Cloud and DevOps`: Basic understanding of cloud platforms (like AWS, Azure, Google Cloud), Docker, Kubernetes, CI/CD pipelines (Jenkins, GitLab, etc.), and version control (Git).

### Behavioral and Soft Skills:
1. `Problem-Solving`: Practice solving coding problems on platforms like LeetCode, HackerRank, or CodeSignal.

2. `Communication`: Be prepared to explain your past projects, technical decisions, and problem-solving approaches clearly.

3. `Teamwork and Collaboration`: Provide examples of working effectively in teams, handling conflicts, or leading initiatives.

4. `Adaptability`: Discuss how you've adapted to new technologies, learned new skills, or handled changing project requirements.

### Interview Tips:
- `Research the Company`: Understand their products/services, culture, and recent news.
  
- `Practice Coding`: Whiteboard or online coding challenges to simulate interview conditions.

- `Ask Questions`: Prepare thoughtful questions about the role, team, projects, or company culture.

- `Review Your Resume`: Be ready to discuss your experience, projects, and any technical achievements in detail.

- `Stay Calm and Confident`: Remember, interviews are as much about how you approach problems as they are about technical knowledge.




👨🏻‍💻  HAPPY CODING !!!!!! 🕶️
