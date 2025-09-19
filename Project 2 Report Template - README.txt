COMP 313/413 Project 2 Report Template

TestList.java and TestIterator.java

	TODO also try with a LinkedList - does it make any difference?

		 yes though the syntax is same, the performance of arraylist and linkedlist would depend on the pattern of the program, if is a large data, Arraylist works better due to its large cache locality and contiguous storage whereas linkedlist performs well when insertions and removal are frequently required at the iterators position and for randon indexing.

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			In arraylist it removes the value at index 5 and returns the removed element and shifts the next elements to the left where as in linkedlist it goes to index 5 and unlinks

		list.remove(Integer.valueOf(5)); // what does this one do?

			Removes the first occurence of the values and returns true if present else false.

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			Threw an error in this case due to an overload.

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.

	SIZE 10
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  val1 val2 val3 val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: val1 val2 val3 val4 val5 val6
		testArrayListAccess:     val1 val2 val3 val4 val5 val6
        testLinkedListAccess:    val1 val2 val3 val4 val5 val6

	SIZE 100
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  val1 val2 val3 val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: val1 val2 val3 val4 val5 val6
		testArrayListAccess:     val1 val2 val3 val4 val5 val6
        testLinkedListAccess:    val1 val2 val3 val4 val5 val6

	SIZE 1000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  val1 val2 val3 val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: val1 val2 val3 val4 val5 val6
		testArrayListAccess:     val1 val2 val3 val4 val5 val6
        testLinkedListAccess:    val1 val2 val3 val4 val5 val6

	SIZE 10000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  val1 val2 val3 val4 val5 val6  ... (fill these in in ms)
        testLinkedListAddRemove: val1 val2 val3 val4 val5 val6
		testArrayListAccess:     val1 val2 val3 val4 val5 val6
        testLinkedListAccess:    val1 val2 val3 val4 val5 val6

	listAccess - which type of List is better to use, and why?

		Arraylist is better because it can allocate more data and is easier than linkedlist also the latter must traverse across nodes to reach the index

	listAddRemove - which type of List is better to use, and why?

		Arraylist is a better option here as well, however if the program requires a lots of iteration Linkedlist can perform well.
