# Memory-in-Logisim
4 bit Memory in logisim


**Steps:**

--> A matrix of d flip flop is made which has dimensions 32X5 which means there are 32 rows
and in each row there are 4 d flip flops.

--> A 5X32 decoder is used. A 5 bit input is given to the decoder as the address to access the row

--> Decoder’s 32 output lines are connected to each flip flops in every rows which will work as
enable.

--> 4 bit input is taken and that input is connected bitwise with flip flops in every rows. Example,
first bit of input is connected to the input of every flip flops in first column.

--> There is a clock input in circuit.

--> For, output a multiplexer is used which has dimensions 32X5.

--> In each row, every bit are combined using a splitter and connected to multiplexer.

--> As the input for selection line the 5 bit input which was given to decoder will be used.

--> Output will be shown from the output of multiplexer.

--> There is also a reset button.


**Working:**

--> Working can be explained easily by using an example like if we want to store “0111” on the
address “10110”.

--> For that we have to give “0111” to input and “10110” to address, this input will then be
provided to every flip flops in every rows.

--> Then enable is changed to one which will pass through decoder and that 23rd row will activate
and when clock pulse is given input “0111” will be stored in the flip flops of 23rd row.

--> Address “10110” is also provided as selection input in multiplexer so, flip flops from 23rd row
will pass output to multiplexer and that will be shown in output.

--> To show any data stored in any row we just need to give address of that row and that stored
data on that row will be displayed on output.

--> Reset button will reset all the flip flops of circuit


**Input:**

--> 4bit input: 4 bit input to store.

--> 5bit input: 5 bit input as an address to store 4bit data

**Output:**

--> 4bit Output: 4 bit output of the data of the row of given address.
