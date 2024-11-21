# CS180 Practice Final Exam - Answer Key

1. A) false, true, true
   - s1 is a new object, so == comparison with s2 is false
   - s2 and s3 are string literals, so they reference the same object
   - equals() compares content, so it's true

2. B) 4
   - The height would be 4 levels: 45 → 23/67 → 12/34/89 → 56

3. B) Fibonacci number at position n
   - The recursive pattern matches Fibonacci sequence calculation

4. C) Sideways order
   - Only preorder, inorder, postorder, and level-order are valid tree traversals

5. A) O(1)
   - LinkedList maintains a tail pointer, making end insertion O(1)

6. B) 18
   - x++ uses current value (5) then increments
   - ++x increments first then uses value
   - Sequence: 5 + 7 + 6 = 18

7. B) Stack
   - Stack's LIFO property naturally supports undo operations

8. B) 0.0
   - Integer division happens first (1/2 = 0), then cast to double

9. C) int[]
   - Primitive arrays have the lowest memory overhead

10. B) Make constructor private and provide public static getInstance() method
    - This is the correct implementation of Singleton pattern

11. B) Throws IndexOutOfBoundsException
    - Java throws this exception for invalid index access

12. B) They can be instantiated directly
    - Abstract classes cannot be instantiated

13. C) ABC
    - try block executes A, catch block executes B, finally always executes C

14. C) LinkedHashSet
    - LinkedHashSet maintains insertion order while HashSet doesn't

15. B) O(log n)
    - Binary search divides the search space in half each time

16. A) 5 3 2 4 7 6 8
    - This is preorder traversal (root, left, right)

17. A) Generic arrays cannot be created directly
    - Java doesn't allow direct creation of generic arrays

18. B) (rear + 1) % capacity == front
    - This is the correct condition for circular queue being full

19. C) udrCS
    - After reverse and operations, "ud" remains with "CS" appended

20. A) They can have private methods as of Java 9
    - Java 9 introduced private interface methods

21. A) 8
    - 12 (1100) & 25 (11001) = 8 (1000)

22. A) Finding minimum element
    - Just follow left pointers to leftmost node

23. A) NotSerializableException is thrown
    - All object references must be serializable

24. A) [1, 3, 3]
    - Final push duplicates the top element (3)

25. B) implements Comparable<Student>
    - Correct way to implement type-safe comparison

26. C) HashSet
    - HashSet provides O(1) lookup for spell checking

27. A) 10
    - Sum sequence: 1 + 2 + 3 + 4 = 10

28. C) Faster insertion/deletion in the middle
    - LinkedList only needs to update references

29. A) System.gc() guarantees immediate garbage collection
    - It's only a suggestion to the JVM

30. A) AB
    - Both exception messages are printed in order

31. A) HashMap with LinkedList
    - Provides O(1) access with order tracking

32. B) 2 4
    - Only prints elements at odd indices

33. C) Overridden methods must have covariant return types
    - This is a requirement for method overriding

34. C) O(n²)
    - Each removal is O(n), done n times

35. C) Inorder
    - Inorder traversal visits nodes in sorted order

36. B) true
    - Type erasure makes them the same class at runtime

37. B) Depth-first search
    - Recursive maze solving implements DFS

38. B) University
    - Arrays.asList creates a view of the array

39. D) values()
    - Must traverse all entries, O(n)

40. C) Compilation error
    - Can't reassign final variable in multiple static blocks

41. B) When the tree becomes a linked list
    - Creates O(n) height instead of O(log n)

42. B) false true
    - Floating point arithmetic isn't exact

43. C) HashMap<String, Integer>
    - Best for counting occurrences

44. A) 321123
    - Recursive concatenation builds this pattern

45. D) Local objects are stored in the stack
    - All objects are stored in heap

46. B) 012
    - Prints 0,1,2 then breaks outer loop

47. C) Both A and B can be used
    - Either interface works for custom comparison

48. C) O(k)
    - Must traverse k nodes to find kth element

49. B) [1, 3]
    - remove(1) removes element at index 1

50. B) An interface can extend multiple interfaces
    - Java allows multiple interface inheritance

51. C) false true
    - intern() returns string pool reference

52. B) O(log n)
    - Balanced BST height is logarithmic

53. C) TreeSet
    - TreeSet maintains natural ordering

54. C) Third error
    - Finally block always executes last

55. B) Make class final and all fields final
    - Required for true immutability

56. B) false
    - 5.0 equals 5.0, so not greater

57. B) Checks moves in sequence, stopping at first success
    - Short-circuit evaluation applies

58. C) ConcurrentModificationException
    - Can't modify list during foreach loop

59. B) Trie
    - Optimal for prefix-based operations

60. A) 5
    - 15 ^ 10 = 5 in binary

61. C) Finding an element by index
    - Requires traversing the list

62. B) 5
    - Default int value (0) plus length (5)

63. D) Multiple threads can run the same Runnable
    - Runnable can be shared between threads

64. B) 12
    - 2*2 + 4*2 = 12

65. A) Two Stacks
    - Optimal for back/forward navigation

66. B) The field is not serialized
    - Static fields belong to class, not instance

67. C) Finding the sum of all elements
    - Requires visiting all nodes

68. C) Hello
    - String is immutable, operations return new strings

69. D) Objects might not be garbage collected even if unreachable
    - GC timing is not guaranteed

70. A) A
    - Nested ternary evaluates to "A"

71. C) Insertion sort
    - Most efficient for nearly sorted data

72. B) [A, C, B]
    - Inserts C at index 1, shifting B

73. D) Interface variables must be static and final
    - This is true, not false

74. A) O(n)
    - Must visit all nodes once

75. A) 32
    - Operations result in printing 3 then 2