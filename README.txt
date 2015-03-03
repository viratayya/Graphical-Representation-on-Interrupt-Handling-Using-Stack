                       Graphical representation of Interrupt handling using stack


Aim: Graphical representation of Interrupt handling in a processor  using stack
Objectives: 
* Interrupt handling with specified Interrupt handlers in a processor using stack.
* Implementing the Interrupts handling graphically.
Introduction:
 Interrupt and handler
      An interrupt is a request of the processor to suspend its current program and transfer control to a new program called the Interrupt Service Routine (ISR). Special hardware mechanisms that are designed for maximum speed force the transfer. The ISR determines the cause of the interrupt, takes the appropriate action, and then returns control to the original process that was suspended.[1]
* In 1954, the NBS DYSEAC was the first one to have an I/O interrupt.[2]
* An interrupt is a change in a execution caused by an external event. [3]
Types of Interrupts [4]:
1. Software Interrupts
2. Hardware Interrupts
3. Exceptions
?	Interrupt handling in a PC:
On a PC there are 24 separate interrupt lines that can be asserted. The appropriate interrupt handler is invoked based on the interrupt number[5].
Interrupt handling – OS ISSUES
?	When an interrupt is serviced the processor must be able to execute without being interrupted. It must have the capability of temporarily disabling the interrupt atomically[6]
?	If an interrupt occurs while an interrupt service is ongoing, it is simply deferred and considered a pending interrupt. It is serviced after the current request terminates[7].

Autodetecting the IRQ Number:[8]
How to get the number? Have the device tells you
MostmoderndevicesannouncetheIRQ#ituses Including PCI devices
The drivers get the IRQ# by reading a status byte from one of the device’s I/O ports or PCI configuration space.

Mechanism:
        When a normal program is running suddenly a interrupt is generated, the value of the program counter is pushed in to the stack then ISR(Interrupt Service routine) will be handling the interrupt in case if there is another interrupt by hardware / software then again the current value of the program counter pushed in to the stack like this there will be a series of interrupts occurs  and those stored in the stack.
             The first interrupt of the stack will be popped and handled by the processor it continues till it executes the first process which we have pushed into the stack.
             This will be shown in a graphical representation.  
System & Software requirements:

?	Software Requirements:

?	Languages  : c++
?	IDE	   :Drop Box
?	OS  	   :windows 7/higher

?	Hardware Requirements:

?	Processor  :Pentium i3/higher
?	RAM	   :  Minimum 1024MB
?	Hard disk  :  Minimum 500GB
