# programming-according-to-os
tophalf and bottom half
first we go with the top halve 
when interrupt occurs the ISR(INTERRUPT SERVICE ROUTINE) is invoked .
from this isr it will go to interrupt descriptor table 
in interrupt descriptor table we have  address and value of register 
the isr checks the address and value of register .
then it goes to interrupt vector table from here it checks the handler and next functions
handler takes the interrupts and completes the task of generated interrupts and sends the high priority interrupts to the bottom halves
bottom halves contains workqueue,tasklet,softirq  
