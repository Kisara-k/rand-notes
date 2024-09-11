# rand-notes

4. If the console was initialized before the thread system, will the outcome change? briefly explain.

Yes

Console in pintos ins responsible for basic I/O, providing fuctions such as printf() and processing keyboard inputs.
In pintos threads run concurrently. Thread system is responsible for managing multiple threads, including scheduling and synchronization.

Initializing the Console before thread system can lead to errors, because thread dependant functions in the console, like one thead waiting to print on the console while another thread prints, require the thread system to function properly.


5. why can C functions like scanf() not be used while taking inputs from the PintOS kernel-level shell? What different approach would you suggest implementing to take inputs (in built-in functions of PintOS are used in this process, mention them)












8. what is the purpose of the magic value used in thread struct?
