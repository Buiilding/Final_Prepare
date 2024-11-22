# CS180 Practice Final Exam
## Purdue University - Object-Oriented Programming in Java
### Time: 180 minutes
### Total Questions: 75

**Instructions:** Select the best answer for each question. Each question is worth equal points.

**1. What will be the output of the following code?**
```java
String s1 = new String("Purdue");
String s2 = "Purdue";
String s3 = "Purdue";
System.out.println(s1 == s2);
System.out.println(s2 == s3);
System.out.println(s1.equals(s2));
```

A) false, true, true

B) false, false, true

C) true, true, true

D) true, false, false

**2. In a binary search tree with elements [45, 23, 67, 12, 34, 89, 56], what would be the height of the tree if elements were inserted in the given order?**

A) 3

B) 4

C) 5

D) 6

**3. Consider the following recursive method:**
```java
public static int mystery(int n) {
if (n <= 1) return 1;
return mystery(n-1) + mystery(n-2);
}
```
**What does this method calculate?**

A) Factorial of n

B) Fibonacci number at position n

C) Power of 2^n

D) Sum of first n natural numbers

**4. Which of the following is NOT a valid way to traverse a binary tree?**

A) Preorder

B) Inorder

C) Sideways order

D) Postorder

**5. What is the time complexity of adding an element to the end of a LinkedList?**

A) O(1)

B) O(n)

C) O(log n)

D) O(n^2)

**6. What will be printed by this code?**
```java
int x = 5;
System.out.println(x++ + ++x + x++);
```
A) 15

B) 18

C) 19

D) 21

**7. Which data structure would be most efficient for implementing an undo feature in a text editor?**

A) Queue

B) Stack

C) ArrayList

D) HashMap

**8. What is the output of this code?**
```java
double result = (double)(1/2) * 8;
System.out.println(result);
```
A) 4.0

B) 0.0

C) 2.0

D) 8.0

**9. In terms of memory usage, which is more efficient?**

A) ArrayList<Integer>

B) LinkedList<Integer>

C) int[]

D) Vector<Integer>

**10. What is the correct way to implement a Singleton pattern in Java?**

A) Make constructor public and static

B) Make constructor private and provide public static getInstance() method

C) Make all methods static

D) Use public final class

**11. What happens when you try to access an index beyond the size of an ArrayList?**

A) Returns null

B) Throws IndexOutOfBoundsException

C) Returns -1

D) Automatically expands the ArrayList

**12. Which statement about abstract classes is FALSE?**

A) They can have constructors

B) They can be instantiated directly

C) They can have both abstract and non-abstract methods

D) They can have static methods

**13. What is the output of this code?**
```java
try {
System.out.print("A");
throw new Exception();
} catch (Exception e) {
System.out.print("B");
} finally {
System.out.print("C");
}
```
A) A

B) AB

C) ABC

D) AC

**14. Which collection type maintains insertion order?**

A) HashSet

B) TreeSet

C) LinkedHashSet

D) All of the above

**15. What is the time complexity of binary search on a sorted array?**

A) O(n)

B) O(log n)

C) O(1)

D) O(n^2)

**16. Given a binary tree implementation, what would be the output of this traversal?**

```java
void traverse(Node root) {
if (root != null) {
System.out.print(root.value);
traverse(root.left);
traverse(root.right);
}
}
```

Tree structure: 
       5
     /   \
    3     7
   / \   / \
  2   4 6   8

A) 5 3 2 4 7 6 8

B) 2 3 4 5 6 7 8

C) 2 4 3 6 8 7 5

D) 5 7 8 6 3 4 2

**17. What is wrong with this code?**
```java
public class MyList<T> {
private T[] elements = new T[10]; // Line 1
private int size = 0;
public void add(T element) {
elements[size++] = element;
}
}
```
A) Generic arrays cannot be created directly

B) T must extend Object

C) size should be static

D) add method needs to be generic

**18. In a queue implementation using a circular array, what is the condition for the queue being full?**

A) front == rear

B) (rear + 1) % capacity == front

C) rear == capacity - 1

D) front == capacity - 1

**19. What will this code print?**
```java
String s = "Purdue";
StringBuilder sb = new StringBuilder(s);
sb.reverse().append("CS").delete(0, 2);
System.out.println(sb);
```
A) druPCS

B) eudrCS

C) udrCS

D) CSPurdue

**20. Which statement about Java interfaces is TRUE?**

A) They can have private methods as of Java 9

B) They can have protected methods

C) They can have static initializers

D) They can have instance variables

**21. What is the output of this bitwise operation?**
```java
System.out.println(12 & 25);
```
A) 8

B) 29

C) 37

D) 13

**22. In terms of time complexity, which operation is most efficient for a balanced BST?**

A) Finding minimum element

B) Finding maximum element

C) Finding average of all elements

D) Finding median element

**23. What happens when you try to serialize an object that contains a reference to a non-serializable object?**

A) NotSerializableException is thrown

B) Only the serializable parts are saved

C) Compilation error

D) Runtime error without exception

**24. Given a Stack implementation, what would be the final state after these operations?**
```java
Stack<Integer> stack = new Stack<>();
stack.push(1);
stack.push(2);
stack.pop();
stack.push(3);
stack.push(4);
stack.pop();
stack.push(stack.peek());
```
A) [1, 3, 3]

B) [1, 3]

C) [1, 3, 4]

D) [1, 4, 4]

**25. What is the correct way to implement the Comparable interface?**

```java
class Student {
private String name;
private double gpa;
}
```

A) implements Comparable

B) implements Comparable<Student>

C) implements Comparable<Object>

D) extends Comparable<Student>

**26. Which collection would be most appropriate for implementing a spell checker?**

A) ArrayList

B) LinkedList

C) HashSet

D) TreeMap

**27. What is the output of this recursive method for n=4?**
```java
public static int mystery(int n) {
if (n == 0) return 0;
if (n == 1) return 1;
return mystery(n-1) + n;
}
```
A) 10

B) 8

C) 6

D) 4

**28. What is the primary advantage of using a LinkedList over an ArrayList?**

A) Faster random access

B) Less memory usage

C) Faster insertion/deletion in the middle

D) Better cache locality

**29. Which statement about Java's garbage collection is FALSE?**

A) System.gc() guarantees immediate garbage collection

B) Objects with no references are eligible for garbage collection

C) finalize() method is called before garbage collection

D) Garbage collection can happen at any time

**30. What will be printed?**
```java
try {
throw new RuntimeException("A");
} catch (Exception e) {
try {
throw new Exception("B");
} catch (Exception e2) {
System.out.print(e.getMessage());
System.out.print(e2.getMessage());
}
}
```
A) AB

B) BA

C) A

D) B

**31. Which data structure would be most efficient for implementing a cache with a "least recently used" eviction policy?**

A) HashMap with LinkedList

B) TreeMap

C) ArrayList

D) Stack

**32. What is the output of this code?**
```java
int[] arr = {1, 2, 3, 4, 5};
for(int i = 0; i < arr.length; i++) {
if(i % 2 == 0) continue;
System.out.print(arr[i]);
}
```
A) 1 3 5

B) 2 4

C) 1 2 3 4 5

D) 24

**33. Which statement about method overriding is TRUE?**

A) Private methods can be overridden

B) Static methods can be overridden

C) Overridden methods must have covariant return types

D) Final methods can be overridden

**34. What is the time complexity of removing all elements from a LinkedList using remove(0)?**

A) O(1)

B) O(n)

C) O(n²)

D) O(log n)

**35. In a binary search tree, which traversal would print the elements in sorted order?**

A) Preorder

B) Postorder

C) Inorder

D) Level-order

**36. What will be the result of this code?**
```java
class Animal { }
class Dog extends Animal { }
class Cat extends Animal { }
public class Test {
public static void main(String[] args) {
ArrayList<Animal> animals = new ArrayList<>();
ArrayList<Dog> dogs = new ArrayList<>();
System.out.println(animals.getClass() == dogs.getClass());
}
}
```
A) false

B) true

C) Compilation error

D) Runtime error

**37. Given a maze solving algorithm using recursion, what type of search does it implement?**

A) Breadth-first search

B) Depth-first search

C) Binary search

D) Linear search

**38. What is the output of this code?**
```java
String[] arr = {"Purdue", "CS", "180"};
List<String> list = Arrays.asList(arr);
arr[0] = "University";
System.out.println(list.get(0));
```
A) Purdue

B) University

C) null

D) ArrayIndexOutOfBoundsException

**39. Which operation is NOT O(1) for a HashMap?**

A) put()

B) get()

C) containsKey()

D) values()

**40. What happens when you try to compile and run this code?**
```java
public class Test {
private static final int x;
private static final int y = 10;
static {
x = 20;
}
static {
x = 30;
}
}
```
A) Compiles and runs, x equals 30

B) Compiles and runs, x equals 20

C) Compilation error

D) Runtime error

**41. In a binary search tree, what is the worst-case scenario for insertion?**

A) When the tree is perfectly balanced

B) When the tree becomes a linked list

C) When the tree has duplicate values

D) When the tree is empty

**42. What will this code print?**
```java
double d = 0.1 + 0.2;
System.out.println(d == 0.3);
System.out.println(Math.abs(d - 0.3) < 1e-10);
```
A) true true

B) false true

C) true false

D) false false

**43. Which collection type would be most appropriate for implementing a unique word counter in a document?**

A) ArrayList<String>

B) LinkedList<String>

C) HashMap<String, Integer>

D) TreeSet<String>

**44. What is the output of this recursive method for n=3?**
```java
public static String mystery(int n) {
if (n == 0) return "";
return n + mystery(n-1) + n;
}
```
A) 321123

B) 123321

C) 333

D) 3213

**45. Which statement about Java's memory model is FALSE?**

A) Objects are stored in the heap

B) Primitive variables in methods are stored in the stack

C) Static variables are stored in the method area

D) Local objects are stored in the stack

**46. What will be printed?**
```java
int i = 0;
outer:
while (true) {
i++;
inner:
for (int j = 0; j < 10; j++) {
if (i > 1) break outer;
if (j > 2) continue inner;
System.out.print(j);
}
}

A) 012012

B) 012

C) 0123456789

D) Infinite loop

**47. Which interface should be implemented to create a custom comparison method?**

A) Comparable

B) Comparator

C) Both A and B can be used

D) Neither A nor B

**48. What is the time complexity of finding the kth smallest element in a BST?**

A) O(1)

B) O(log n)

C) O(k)

D) O(n)

**49. What will happen when this code is executed?**
``` java
Queue<Integer> queue = new LinkedList<>();
queue.add(1);
queue.add(2);
queue.add(3);
queue.remove(1);
System.out.println(queue);
```
A) [2, 3]

B) [1, 3]

C) [1, 2]

D) [1, 2, 3]

**50. Which statement about abstract classes and interfaces is TRUE?**

A) A class can implement multiple abstract classes

B) An interface can extend multiple interfaces

C) Abstract classes can have final methods

D) All of the above

**51. What is the output of this code?**
```java
String s1 = "Hello";
String s2 = new String("Hello");
String s3 = s2.intern();
System.out.println(s1 == s2);
System.out.println(s1 == s3);
```
A) true true

B) false false

C) false true

D) true false

**52. In a balanced binary search tree with n nodes, what is the height?**

A) O(n)

B) O(log n)

C) O(n²)

D) O(1)

**53. Which collection maintains elements in sorted order?**

A) HashMap

B) LinkedHashSet

C) TreeSet

D) HashSet

**54. What will be the result of this operation?**
```java
try {
throw new Exception("First");
} catch (Exception e) {
throw new RuntimeException("Second");
} finally {
throw new Error("Third");
}
```
A) First exception

B) Second exception

C) Third error

D) All exceptions in sequence

**55. What is the correct way to create an immutable class?**

A) Make all fields private

B) Make class final and all fields final

C) Make all methods synchronized

D) Make all fields static

**56. What will be the output of this code involving generics?**
```java
class Box<T extends Number> {
T value;
Box(T value) { this.value = value; }
boolean isGreater(Box<? extends Number> other) {
return this.value.doubleValue() > other.value.doubleValue();
}
}
public class Test {
public static void main(String[] args) {
Box<Integer> b1 = new Box<>(5);
Box<Double> b2 = new Box<>(5.0);
System.out.println(b1.isGreater(b2));
}
}
```
A) true

B) false

C) Compilation error

D) Runtime error

**57. In a maze solving algorithm, what does the following code accomplish?**
```java
if (solve(row-1, col) || solve(row+1, col) ||
solve(row, col-1) || solve(row, col+1))
return true;
```
A) Checks all possible moves simultaneously

B) Checks moves in sequence, stopping at first success

C) Always checks all four directions

D) Returns true regardless of move success

**58. What is the output when trying to remove elements while iterating?**
```java
ArrayList<Integer> list = new ArrayList<>(Arrays.asList(1, 2, 3, 4));
for(Integer num : list) {
if(num % 2 == 0) {
list.remove(num);
}
}
```
A) [1, 3]

B) [1, 2, 3, 4]

C) ConcurrentModificationException

D) [2, 4]

**59. Which data structure would be most efficient for implementing a spell checker that needs to suggest similar words?**

A) HashMap

B) Trie

C) Binary Search Tree

D) LinkedList

**60. What is the result of this bitwise operation?**
```java
System.out.println(15 ^ 10);
```
A) 5

B) 25

C) 150

D) 0

**61. In terms of time complexity, which operation is most expensive for a LinkedList?**

A) Adding to the beginning

B) Adding to the end

C) Finding an element by index

D) Removing from the beginning

**62. What will this code print?**
```java
int[] arr = new int[5];
System.out.println(arr[0] + arr.length);
```
A) 0

B) 5

C) null5

D) NullPointerException

**63. Which statement about Java threads is TRUE?**

A) A thread can be started multiple times

B) Thread priorities guarantee execution order

C) Thread.sleep() releases all locks

D) Multiple threads can run the same Runnable

**64. What is the output of this code using streams?**
```java
List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5);
int sum = numbers.stream()
.filter(n -> n % 2 == 0)
.map(n -> n 2)
.reduce(0, Integer::sum);
System.out.println(sum);
```
A) 30

B) 12

C) 15

D) 6

**65. Which collection would be most appropriate for implementing a browser's back/forward functionality?**

A) Two Stacks

B) Single Queue

C) ArrayList

D) LinkedHashMap

**66. What happens when you try to serialize a static field?**

A) The field is serialized normally

B) The field is not serialized

C) Compilation error

D) SerializationException is thrown

**67. In a binary search tree, what operation would require a tree traversal?**

A) Finding minimum element

B) Finding maximum element

C) Finding the sum of all elements

D) Finding a specific element

**68. What will be printed?**
```java
String str = "Hello";
str.concat(" World");
str.toUpperCase();
System.out.println(str);
```
A) Hello World

B) HELLO WORLD

C) Hello

D) HELLO

**69. Which statement about Java's memory management is TRUE?**

A) System.gc() guarantees memory cleanup

B) finalize() is called exactly once

C) Memory leaks are impossible

D) Objects might not be garbage collected even if unreachable

**70. What is the output of this code?**
```java
int x = 5;
System.out.println(x > 3 ? x < 10 ? "A" : "B" : "C");
```
A) A

B) B

C) C

D) Compilation error

**71. Which sorting algorithm would be most efficient for sorting a nearly-sorted array?**

A) Quicksort

B) Mergesort

C) Insertion sort

D) Selection sort

**72. What will happen when executing this code?**
```java
List<String> list = new ArrayList<>();
list.add("A");
list.add("B");
list.add(1, "C");
System.out.println(list);
```
A) [A, B, C]

B) [A, C, B]

C) [C, A, B]

D) IndexOutOfBoundsException

**73. Which statement about Java interfaces is FALSE?**

A) An interface can extend multiple interfaces

B) Interface methods are public by default

C) Interfaces can have private methods as of Java 9

D) Interface variables must be static and final

**74. What is the time complexity of finding the diameter of a binary tree?**

A) O(n)

B) O(log n)

C) O(n²)

D) O(h) where h is height

**75. Given a Stack implementation, what would be the output?**
```java
Stack<Integer> stack = new Stack<>();
stack.push(1);
stack.push(2);
stack.push(3);
System.out.print(stack.pop());
stack.push(stack.peek());
System.out.print(stack.pop());
```
A) 32

B) 33

C) 23

D) 22

