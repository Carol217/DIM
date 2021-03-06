# DIM
Team Dim (Mansour Elsharawy, Dawei Huang, Irene Lam)

## Class Deque
Interface short for "double ended queue" in which methods allow users to access elements on either end of the deque.

**Rationale (use of ArrayList<T> class)**

     ArrayList<T> is much simpler in structure than a set of doubly-linked nodes,
     and while wiring the code for the Deque inteface with an ArrayList may need linear
     runtime for methods that a doubly-linked node can otherwise handle in constant time,
     using an ArrayList has a lot less room for mistakes than a doubly-linked list by not having to deal
     with all of the pointers and having to manage a _front and _end pointer.

**Method Explanations**
1. void addFirst(T e) - adds an element to the front of the deque
2. void addLast(T e) - adds an element to the end of the deque
3. T removeFirst() - removes the element at the front of the deque
4. T removeLast() - removes the element at the end of the deque
5. T peekFirst() - returns the element at the front of the deque
6. T peekLast() - returns the element at the end of the deque
7. int size() - returns the size of the deque
8. boolean isEmpty() - returns true if the deque is empty and false otherwise
9. String toString() - returns a String representation of the deque from front to end

**Why We Chose Our Methods**

     toString() is the most obvious method to include, because every class
     created should have a way of representing itself in a String format.
     As for isEmpty(), that method can be very useful for handling situations
     such as what to do if a removal is attempted on an empty deque.
     The addFirst() and addLast() methods are instrumental in adding elements
     to either end of the deque, similar to adding methods in a queue or stack.
     removeFirst() and removeLast() are also the simplest implementations of
     removing an element from either end of the deque while returning that
     element as well, just like a queue or stack, and the same goes for
     peekFirst() and peekLast(). We didn't bother covering other methods
     such as pollFirst() or pollLast() because we feel that the basic ones
     already have the same function and doing those as well would just be redundant.
