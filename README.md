# FPGA-Matrix-Engine
The matrix unit will perform matrix multiplication, scaler multiplication, subtraction, addition,  and transposition. 
A testbench will place a starting set of matrix in RAM. It will also place the opcodes for the execution unit to perform the matrix functions using the matrix modules. 
All math functions will have a clear input to set it to 0. 
The Register value needs to be able to be written back into a memory location
All Matrices will be 4x4 16 bit deep.
Matrix multiplier will multiple two 4x4 matrix and return a 4x4 matrix
Scalar multiplication is multiplying a matrix by a single number
Add and Subtract will add and subtract 2 4x4 matrix
Transpose will flip a matrix along its diagonal. 
Load 2 matrix’s into RAM
Load opcodes into RAM for the execution unit.

Operations to be performed
Add the first matrix to the second matrix and store the result in memory.
Subtract the first matrix from the result in step 1 and store the result somewhere else in memory. 
Transpose the result from step 1 store in memory
Scale the result in step 3 store in a register
Multiply the result from step 4 by the result in step 3, store in memory. 

The test bench will place the starting matrixes in memory and toggle reset
Execution engine will fetch the first opcode from memory and begin execution.
The execution engine will direct the transfer of data between the memory, the appropriate matrix modules and memory. 
The execution engine will continue executing programs until is finds a STOP opcode.
The test bench will instantiate ALL models and create an output waveform to determine correct operation. The test bench will ALSO provide the system clock as well as the number of clock cycles required to complete the tasks.

Matrix Addition  to/from memory, to/from register
Matrix Subtraction  to/from memory, to/from register
Matrix Multiply  to/from memory, to/from register
Matrix Transpose to/from memory, to/from register
Matrix scale  to/from memory, to/from register

