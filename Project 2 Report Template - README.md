COMP 313/413 Project 2 Report Template

TestList.java and TestIterator.java

	TODO also try with a LinkedList - does it make any difference?

		-No. They behave about the same in terms of what they do.

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			Removes element at index 5

		list.remove(Integer.valueOf(5)); // what does this one do?

			Removes the first 5 that pops up

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			Throws exception because of list modification iteration

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.
	These are examples of SIZEs you might choose, you can choose others if you wish.

	SIZE 10
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  14 16 15   ... (fill these in in ms)
        testLinkedListAddRemove: 11 15 12
		testArrayListAccess:     7 8 7 7
        testLinkedListAccess:    6 7 7

	SIZE 100
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  23 23 23 ... (fill these in in ms)
        testLinkedListAddRemove: 11 13 10
		testArrayListAccess:     7 13 9
        testLinkedListAccess:    16 16 10

	SIZE 1000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  151 145 148   ... (fill these in in ms)
        testLinkedListAddRemove: 12 12 11
		testArrayListAccess:     9 8 7
        testLinkedListAccess:    315 318 315

	SIZE 10000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  1.513s 1.511s  ... (fill these in in ms)
        testLinkedListAddRemove: 14 11
		testArrayListAccess:     20 8
        testLinkedListAccess:    4.238s 4.260s

	listAccess - which type of List is better to use, and why?

		ArrayList is much better when dealing with size that scales. Better time complex.

	listAddRemove - which type of List is better to use, and why?

		LinkedList is much better regardless of size. Better removal time complex.
