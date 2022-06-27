# Center_of_Gravity_RAM
Small algorithm that will return the "center of gravity" of a data stream stored in the internal RAM of the circuit.

This project is looking to calculate the center of gravity of a 16 item-long data stream. The algorithm is implemented in the Verilog HDL, as part of a practical examination for the "Integrated Digital Circuits" course. 

We define "center of gravity" as 'g'. 'g' is a simple integer that represents the point of the stream where the sum of the first g inputs is smaller than the rest of the data stream inputs AND the sum of the g+1 inputs is smaller than the sum of the remaining inputs. In essence, we shall imagine a steel lifting bar. Should we lift this bar, we will pick it up from the middle, it's center of gravity. Considering that we add weights all around the length of the bar and try to lift it from the middle, we are not 100% certain the weight ballance is equal. This example perfectly sums up the role of this project. 

The data stream inputed will be stored in a RAM module only at the impulse of the start input. Following a couple of seconds, while the algorithm is working, we will discover at output the 'valid' impulse along with the 'g' value. 

This project is composed of the 'RAM' module that is declared inside of the 'gravity' module, simulating it in a simple test bench, under the 'gravity_tb" file.

The circuit is a work-in-progress.
