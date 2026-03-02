# SSU-CS-351
Computer Architecture with Dave
* Project 1 - Analysis & Reporting
1. Which program is fastest? Is it always the fastest?
    <p>Of the programs, alloca.out seems to rank the fastest though only when the optional arguments (MIN_BYTES, MAX_BYTES, NUM_BLOCKS) are at mid to high values otherwise the fastest gets hard to determine because the variations in each trail leads to similar time averages. But noticebly the lower the NUM_BLOCKS value the better malloc.out seems to perform, ever so slightly. So while alloca.out is generally the fastests, plenty of different trials show that it's not always the case.</p>
2. Which program is slowest? Is it always the slowest?
    <p>The slowest is somewhat difficult to dictate but I'd say it'd be list.out if only for the fact that it generally has the largest max time value out of all the programs. It's rather inconsistent in its averages sometimes slowest, sometimes just average, but one thing that is pretty consistent in the trials I did was that the longest time belonged to list, which I think would be the closest to 'the slowest' title.</p>
3. Was there a trend in program execution time based on the size of data in each Node? If so, what, and why?
    <p>Of course, as the greater the size of the data in each Node, the longer the program execution time became. This could be attributed to just how much memory would need to be allocated for each Node when the size of the data was increased.</p>
4. Was there a trend in program execution time based on the length of the block chain?
    <p>Yes, and I'd say the length of the block chain had the greatest impact in program execution time as each 0 I added to the length of the block chain would lead to exponentially increasing run times.</p>
5. Consider heap breaks, what's noticeable? Does increasing the stack size affect the heap? Speculate on any similarities and differences in programs?
    <p>For heap breaks, the greater the stack size, the further up the heap break would be moved/have more memory allocated. And while this can lead to changes, inbetween programs, the differences are minimal. The values are different between programs but very minimally, likely because each program is doing the same thing just differently, so the memory they need is the same.</p>
6. Considering either the malloc.cpp or alloca.cpp versions of the program, generate a diagram showing two Nodes. Include in the diagram
    * the relationship of the head, tail, and Node next pointers.
    * show the size (in bytes) and structure of a Node that allocated six bytes of data
    * include the bytes pointer, and indicate using an arrow which byte in the allocated memory it points to.
    ![My Diagram that is not working for whatever reason, yaya](/Project-1_diagram?.png)
7. There's an overhead to allocating memory, initializing it, and eventually processing (in our case, hashing it). For each program, were any of these tasks the same? Which one(s) were different?
    <p>I'd say the allocation of memory was different for each program, either it functioned on the stack or heap. Though the processing was the same for everyone, considering that each program is doing essentially the same thing just slightly different. Same with initialization.</p>
8. As the size of data in a Node increases, does the significance of allocating the node increase or decrease?
    <p>I think the significance of allocating the Node decreases. If the size of daata in a <i>single</i> Node increases then yes it's significance would increase as comparitively it is considerably more memory that needs to be allocated. But if the size of data in all the Nodes is increasing similarly, then to the total work, no, its not very significant.</p>
