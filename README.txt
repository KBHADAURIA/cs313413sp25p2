TestList.java and TestIterator.java



		Your answer here. Yes it makes difference while Switching between ArrayList and LinkedList can alter the behavior and performance,
		but method functionality remains unchanged as both implement the List interface.

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			Your answer here. list.remove(5) method removes the element of index 5 in the list, not the value 5.
			It does not remove the number 5 from the list but removes the element of index 5.



		list.remove(Integer.valueOf(5)); // what does this one do?

			Your answer here. list.remove(Integer.valueOf(5)) mathod removes the first occurrence of 5th value in the
			 list, not the element of index 5.

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			Your answer here. list.remove(77) method will try to eliminate or remove the first occurrence of the value 77 from the list.

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.
	These are examples of SIZEs you might choose, you can choose others if you wish.
    Note- when I run the code for 4th and 5th time I changed the index number in the code
	SIZE 10
								  #1          #2           #3           #4             #5            #6 	             (as many tests as you ran)
        testArrayListAddRemove:  17.981916ms  17.608416ms  17.56225ms   18.1715ms     19.288541ms   20.692375ms           (fill these in in ms)
        testLinkedListAddRemove: 17.779667ms  18.654292ms  17.558209ms  19.189584ms   19.311625ms   18.495708ms
		testArrayListAccess:     6.868916m    1.34025 ms   4.098667ms   4.073167 ms    4.842083ms    4.68275ms
        testLinkedListAccess:    1.383ms      6.83575 ms   7.01175ms    6.561542ms     7.739334ms    6.76525ms

	SIZE 100
								  #1            #2          #3           #4            #5          #6 	...    (as many tests as you ran)
        testArrayListAddRemove:  24.359125ms    24.732416ms 25.229167ms  26.005125ms  24.620708ms   23.987334ms   (fill these in in ms)
        testLinkedListAddRemove: 13.368167ms    13.25375ms  13.635792ms  13.477125ms  13.535792ms   13.167917ms
		testArrayListAccess:     1.543833ms     1.536333ms  1.538459ms   1.529541ms    1.534709ms    1.535959ms
        testLinkedListAccess:    5.417708ms     5.223625ms  5.270666ms   5.160375ms    5.300416ms    4.924959ms

	SIZE 1000
								  #1              #2         #3            #4            #5            #6 	           (as many tests as you ran)
        testArrayListAddRemove:  144.372375ms    43.697625ms 149.516792ms 163.021875ms   146.045958ms  149.410917ms   (fill these in in ms)
        testLinkedListAddRemove: 9.297416ms      9.180667ms  9.154625ms   9.567792ms     9.416125ms    9.04475ms
		testArrayListAccess:     1.489875ms      1.537959ms  1.605333ms   1.586833ms     1.557291ms     1.517125ms
        testLinkedListAccess:    2.592708ms      2.669292ms  3.207708ms   2.841875ms     2.982041ms      2.99775ms

	SIZE 10000
								  #1             #2            #3             #4              #5            #6 	...       (as many tests as you ran)
        testArrayListAddRemove:  1480.452667ms   1491.304667ms 1492.882417ms  1474.846458ms  1497.255ms   1493.654166ms    (fill these in in ms)
        testLinkedListAddRemove: 10.730625ms     10.987542ms   11.136209ms    10.567042ms    10.307792ms  10.397375ms
		testArrayListAccess:     1.572458ms      1.501791ms    1.569792ms      1.524125ms    1.514333ms    1.488625ms
        testLinkedListAccess:    2.715792ms      2.673042ms    2.976042ms      2.749083ms    2.997667ms    2.706458ms

	listAccess - which type of List is better to use, and why?

		Your answer here. ArrayList is better to use for list access because ArrayList have constant time access for any element in the list.

	listAddRemove - which type of List is better to use, and why?

		Your answer here. LinkedList is better to use for Add/Remove process because LinkedList have constant time for add/remove for any element in the list.