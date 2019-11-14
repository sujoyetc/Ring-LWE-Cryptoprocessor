The cryptoprocessor encrypts a 256-bit message which is split in two parts:
`define message_input_part2 128'b00101111011100000001111101010101111100001110000000101011011001101011010001001000000101000111101010111111110010010001111000111010
`define message_input_part1 128'b01101001000110101111010100011101011101100111001110000010001111111011001010111000000000110001010101001101110011111100111111011101

After completion of the encryption operation, the cryptoprocessor also performs a decryption operation using 
the secret key r2. After the completion of the decryption operation, decrypted message bits are read as in pairs.

The HDL codes have been simulated using Xilinx ISM simulator. 

NOTE: 
	1. The top source file is emulator.v
	   This file emulates a microprocessor and performs data/instruction transfer with the RLWE-Processor.

	2. For area and timing report, please compile the ring-LWE coprocessor part (not the emulator.v).

	3. The processor has several IPCore generated files. Depending on the version of the ISE tool, you
	   may have to regenerate the core files again. 
	   
For questions please contact Sujoy Sinha Roy, KU Leuven (Sujoy.SinhaRoy@esat.kuleuven.be).
	   
