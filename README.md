# VHDL_PeakDetector

Author: [Data Processor: Elim Kwan], [Command Processor: Trevor Leung, Yasin Abughrara]

Date Created: May 2018

Description: The peak detector will process a number of words as typed in by the user in the terminal, and return the peak byte along with the three bytes that precede and follow it in the sequence. It also returns the index of the peak byte in the sequence. The design can be implemented on the Nexys 3 development board with a Spartan 6 device running on a 100 MHz clock. There are 3 supplied modules: a Receiver and Transmitter that implement the RS232 protocol, a Data Generator that supplies a byte at a time under the control of a 2-phase handshaking protocol. The code could be implemented on FPGAs with Xilinx ISE. 


Data Processor: analyses certain number of bytes from the Data Generator and outputs the peak byte of the sequences; with the three bytes before and after the peak, as well as the index of the peak byte.

Command Processor: handle the command input by user.

ANNN (NNN are 3 decimal digits): Start command to process NNN bytes of data. Print each byte processed.

L: Print the 3 bytes preceding the peak, the peak byte itself and the 3 bytes following the peak in the order received. Example output: “09 FA A0 FD BC 10 DE”.

P: Print the peak byte, and the peak index
Example output: “FD 197”.

Push button BTNU (reset): Initialise the system when pressed at any point.
