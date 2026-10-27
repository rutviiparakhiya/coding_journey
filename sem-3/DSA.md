DSA - data structure and algorithem  

▢ Time complexity - it is the amount of time an algorithm takes to solve a problem as the input size increases.   
▢ Space complexity - it is the amount of extra memory an algorithm uses while solving a problem.   

◯ Data structure : It is the way to organize & store data so it can be accessed, updated, and managed efficiently.   
&nbsp;&nbsp;&nbsp;&nbsp; → There are two types of data structure :   
1. primitive : Built-in types (int, char, float, double, bool)   
2. non-primitive : Built using primitive types   

▢ Linear data struture :- Linear data structures store elements in a sequence, one after another.   
→ Each element is connected to the next or previous element.    
e.g. - Array, Linked List, Stack, Queue   

▢ Non-linear data structure :- Data elements are not arranged in a single, sequential order is called non-linear data structure.  
e.g. - trees, graphs   

◯ Algorithem : it is a step-by-step procedure to solve a problem or perform a task.    
e.g. - searching algo, sorting algo, recursion, dynamic programing    

◯ Array :- An array stores multiple values of the same datatype in continuous memory.    
→ Useful when fast, random access is a priority.  

▢ Array Operations and Methods :     
1. Accessing Elements - Retrieve the value at a given index.  
2. Traversing an Array - Visit each element, usually to process or print.  
3. Inserting Elements - Insert a new element at a specific position by shifting subsequent elements.  
4. Deleting Elements - Remove element at a specific index and shift remaining elements left.  
5. Searching Elements (Linear Search) - Find index of an element by checking each position sequentially.  
6. Updating Elements - Change the value at a specific index.
7. Copying Arrays - Create a duplicate array.
8. Resizing Arrays - When array size limit reached, allocate larger array and copy elements.

▢ Advantages of Arrays : 
1. Constant-time access to any element.
2. Simple and efficient for fixed-size data.
3. Supports bulk operations like sorting.

▢ Disadvantages of Arrays :
1. Fixed size limits flexibility.
2. Costly insertions/deletions in middle due to shifts.
3. Inefficient with dynamic, growing data.

▢ Time complexity : 
| operation | time complexity |
| :---------: | :---------------: |
| access    | O(1)            |
| Traverse  | O(n)            |
| insert    | O(n)            |
| delete    | O(n)            |
| search    | O(n)            |
| update    | O(1)            |

◯ String :- It is a sequence of characters used to represent text, such as a name, a word, a sentence, or a message.  

▢ Comman string operations : 
| operation                  | description                           | function/ methods     | typical complexity |
| :--------------------------: | :-------------------------------------: | :---------------------: | :------------------: |
| concatination              | Join strings end-to-end               | +, .append()          | O(m+n)             |
| comperison                 | Check equality or lexicographic order | ==, <, .compare()     | O(n)               |
| substring extraction       | Extract portion of string             | .substr(pos, len)     | O(len)             |
| searching                  | Find substring or character           | .find(), .rfind()     | O(n)               |
| length                     | Get string length                     | .length(), .size()    | O(1)               |
| append                     | Add string or character at the end    | .append(), +=         | O(1)               |
| insertion                  | Insert into string at position        | .insert(pos, str)     | O(n)               |
| replacement                | Replace a part of the string          | .replace(pos,len,str) | O(n)               |
| Conversion (string to int) | Parse string as integer               | stoi(), stol()        | O(n)               |
| Conversion (int to string) | Convert integer to string             | to_string()           | O(logn)            |

◯ Linked List - It is a linear and dynamic data structure consisting of nodes, where each node contains data and a reference to the next node.
→ There are 3 types of linked lists : 
1. Singly Linked List : Nodes have a single pointer to the next node and the last node points to NULL indicating the end of the list.

▢ operations with algorithems :   
(a) Insertion :- Insertion at Beginning, Insertion at End, Insertion at Given Position
(b) Deletion :- Deletion from Beginning (Head), Deletion from End, Deletion at Given Position
(c) Searching :- It means finding whether a given value (key) exists in the Linked List or not.  
(d) Traversal :- It means visiting each node of the Linked List one by one and printing its data.  

2. Doubly Linked List : Nodes have pointers to both next and previous nodes, each node contains three fields: Prev, Data, and Next. It allows traversal in both forward and backward directions.

▢ operations :   
(a) Insertion :- Insertion at Beginning, Insertion at End, Insertion at Given Position
(b) Deletion :- Deletion from Beginning (Head), Deletion from End, Deletion at Given Position
(c) Searching :- It is the process of traversing a Doubly Linked List to find a given key and return its index if found; otherwise, it returns -1.
(d) Traversal(Both functions only print the data and do not return any value because their return type is void) :- It means visiting each node one by one so that its data can be read, printed, or processed. 
→ There ae 2 types of travesal in doubly linked list - forward and backward. 

3. Circular Linked List : It is a linked list in which the last node points back to the first node instead of pointing to NULL.

▢ operations :   
(a) Insertion in an Empty List :- When a Circular Linked List is empty and we insert the first node into it, it is called Insertion in an Empty List.
→ Insertion at Beginning, Insertion at End, Insertion at Given Position.
(c) Delete Node by Key :- While deleting a node, first find the node, then update the next pointer of the previous node, update last if the last node is being deleted, and finally delete the node.
(d) Searching :- It is the process of checking each node's data, starting from the head, until the key is found or traversal returns to the starting node.
(e) traversal :- Traversal means visiting each node of the Linked List one by one and printing its data.

◯ Stack(LIFO) - It is a linear data structure that follows the Last-In, First-Out principle, which means the last element inserted is the first element to be removed.
→ A stack allows insertion and deletion of elements only from the top.

▢ operations : 
1. push - It means inserting a new element at the top of the Stack.   
2. pop - It means removing the element at the top of the Stack and returning its value.

▢ applications of stcak :   
1. Expression Evaluation - It means calculating a mathematical expression to obtain its final answer.
2. Expression Conversion - It means the process of converting a mathematical expression from one notation to another.
→ There are 3 types of conversions :-  
(a) infix : 
(b) prefix :
(c) postfix :