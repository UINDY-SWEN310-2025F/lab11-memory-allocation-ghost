#put your answers here

to-do1-1
 	- The meaning of si is what is swapped in, so - depends on the specific context of the command it is a abbreviation, bi means the blocks in which represents the number of blocks received from a block devices (reads) per second , bo columns stands for blocks out (per second), indicates the amount of data being written to a block device
 	
 to-do2-1 

		- The memory layout shows a series of address intervals, each representing either an available or an occupied partition. To determine the size of each available partition, we subtract the starting address from the ending address. This yields the following free-space sizes: from 600000 to 600200 the size is 200 MB; from 600200 to 600300 the size is 100 MB; from 600300 to 600700 the size is 400 MB; from 600700 to 600800 the size is 100 MB; from 600800 to 601000 the size is 200 MB; from 601000 to 602300 the size is 1300 MB; from 602300 to 602800 the size is 500 MB; from 602800 to 603100 the size is 300 MB; from 603100 to 603400 the size is 300 MB; and from 603400 to 603650 the size is 250 MB. In the memory table you drew, some of these partitions are marked as occupied, meaning they cannot be used to place new processes, while all unoccupied partitions are available for allocation.

 to-do2-2
 		- Using the First-Fit algorithm, each incoming process is compared to the free partitions in order from top to bottom. First-Fit assigns a process to the first partition large enough to hold it, skipping any partition that is either too small or marked as occupied. The list of processes provided—P1 of size 352 MB, P2 of size 210 MB, P3 of size 463 MB, and P4 of size 491 MB—is evaluated against this sequence of partition sizes. You then compared each process with the available free spaces to determine where each process would fit according to First-Fit rules.

 to-do2-3
 		- The issue I see in chart 1 and chart 2 is that the size of p1 and p2 aren't occupied and they are too small because their difference between the occupied and available aren't the same. Other issues practical issues with First-Fit are it tends to leave large gaps early or mid memory depending on order, can produce large internal fragmentation for some processes. Also at the end their tends to be external fragmentation meaning their is unusable free space issues. 

 to-do3-1 
 		- The number of memory frames for 64 bit machine with 16 terabytes RAM usinng 4kb page size is 4,294,967,296 memory frames in total.

	    A 64-bit machine with 16 terabytes of RAM and a 4 KB page size can have its number of memory frames calculated by dividing the total physical memory by the size of each page. Sixteen terabytes is equal to 16*2^40 = 2^44 bytes, and the 4 KB page size is 4*2 = 2^12 bytes. Dividing the total memory by the page size gives 2^44 / 2^12 = 2^32 frames. 

to-do3-2
		12 bits are needed for the displacement into a page. The reason why is because it must be large enough to uniquely identify every byte inside a single page. Page is 4 KB we convery size to power of 2. So 4KB = 4 * 2^10 = 2^12 bytes 

to-do3-3 
		For large like this we need to calculate the virtual memory by multiply the terabytes ram using 4kb with how much bit it takes which is 36 bits. 

		So the calculation would be virtual address = vits + offset bits
		then we have virtual address size = 36 + 12 = 48 bits, then the total size of virtual memory is 2^48 bytes. We need to compute that in order to get the virtual memory size which is 256 terabytes.
