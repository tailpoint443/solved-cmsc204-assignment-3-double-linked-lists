Download Link: https://assignmentchef.com/product/solved-cmsc204-assignment-3-double-linked-lists
<br>
Your assignment is to write a generic double singly-linked list class with an iterator, and a generic sorted double singly-linked list class with an iterator that inherits from your generic double singly-linked list class. The GUI has been provided for you for this assignment to help you visualize your linked list. Your list classes will also be tested with Junit tests. Upload the initial files from Blackboard and your working files in a directory into the repository in GitHub you created in Lab 1 and take a screen shot of the files.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Concepts tested by this assignment</strong></td>

  </tr>

 </tbody>

</table>




Exception handling

Generic Classes

Double Linked List

Ordered Double Linked List

Iterators

Comparators

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Classes</strong></td>

  </tr>

 </tbody>

</table>

<strong>BasicDoubleLinkedList</strong>

This generic double singly-linked list relies on a head (reference to first element of the list) and tail (reference to the last element of the list). Both the head and the tail are set to null when the list is empty. Both point to the same element when there is only one element in the list, and now the element’s “next” and “previous” references point to null. A node structure has only two fields: data and the next references. The class must only define the following entities: an inner class Node, an inner class that implements ListIterator (for the iterator method), head and tail references and an integer representing the list size. However only the next(), hasNext(), previous() and hasPrevious() methods of the ListIterator are you required to implement.  The rest of the methods can throw the UnsupportedOperationException, such as:

public void remove() throws UnsupportedOperationException{

throw new UnsupportedOperationException();}

All the entities are defined as protected so they can be accessed by the subclass.  Follow the Javadoc that is provided.

<strong>SortedDoubleLinkedList</strong>

A generic sorted double linked list will be constructed using a provided Comparator to determine how the list is to be sorted.  It extends BasicDoubleLinkedList class.  The <strong>addToFront</strong> and the <strong>addToEnd </strong>methods will not be supported and an <strong>add</strong> method will be added that inserts to the double linked list in sorted order dependent on the Comparator. Follow the Javadoc that is provided.

<strong>Exception Handling</strong>

<ul>

 <li>UnsupportedOperationException – this exception is a Java library exception and will be returned by the addtoFront and addToEnd implementations of the SortedDoubleLinkedList class and by the remove method of the iterator.</li>

 <li>NoSuchElementException – this exception is a Java library exception and will be returned by the next function within the iterator class when there are no more elements in the linked list.</li>

</ul>

<strong>GUI driver (provided for you)</strong>

<strong>          </strong>A GUI driver has been provided for you to help you visualize your doubly-linked lists. Here is the minimum that must be in place to start using the GUI driver effectively.

<ul>

 <li>All methods in your BasicDoubleLinkedList and SortedDoubleLinkedList must be stubbed.</li>

 <li>The <strong>addToFront</strong> or <strong>addToEnd</strong> method of the BasicDoubleLinkedList must be implemented to create a basic double singly-linked list.</li>

 <li>The <strong>add</strong> method of the SortedDoubleLinkedList must be implemented to create a sorted double singly-linked list.</li>

 <li>The <strong>toArrayList</strong> method in both the BasicDoubleLinkedList and SortedDoubleLinkedList, which returns an arraylist of the items in the list from the head of list to the tail of list. This method is used to display the contents of the lists.</li>

</ul>

<strong>Testing</strong>

<ol>

 <li>Your code should cause the BasicDoubleLinkedList_Test tests to succeed.</li>

 <li>Your code should cause the SortedDoubleLinkedList_Test tests to succeed.</li>

 <li>Create a JUnit Test – Basic</li>

 <li>Create a JUnit Test – SortedDoubleLinkedList_STUDENT_Test.</li>

</ol>

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Examples using GUI driver</strong></td>

  </tr>

 </tbody>

</table>




Adding to a Basic List                                                                                   Adding to a Sorted List

Removing Second from basic                                               Removing Thomas from sorted

start the iterators for Basic and Sorted. Think of iterators being “in between” nodes.

<table width="100%">

 <tbody>

  <tr>

   <td></td>

  </tr>

 </tbody>

</table>

Example of selecting “Next” for Basic and then for Sorted list. Think of iterators being “in between” nodes.

Example of “Next” for basic and “Previous” for Sorted. Think of iterators being “in between” nodes.


