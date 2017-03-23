# Source Files for manialib

## Notes

- Code: The code you find in the .osu format
- Value: The actual value for that parameter

- Eg. SV Code = -10; SV Value = 10
- Eg. BPM Code = 600; BPM Value = 100

- S: Singular
- M: Multiple

**.BPM_CtoV:**  

- Converts BPM Value to Code
- Input (Double) Value
- Return (Double) Code

**.BPM_VtoC:** 

- Converts BPM Code to Value
- Input (Double) Code
- Return (Double) Value
	
**.SV_CtoV:**

- Converts SV Value to Code  
- Input (Double) Value  
- Return (Double) Code  

**.SV_VtoC:**

- Converts SV Code to Value  
- Input (Double) Code  
- Return (Double) Value  

**.Compiler_NN:**

- Compiles parameters into single notes
- Input (Int) Number of Keys, (Int) Key of note, (Double) Offset, (Optional String) Extension
- Return NIL
  
**.Compiler_NL:**

- Compiles parameters into long notes
- Input (Int) Number of Keys, (Int) Key of note, (Double) Start Offset, (Double) End Offset, (Optional String) Extension
- Return NIL

**.Compiler_T:**

- Compiles parameters into a Timing Point
- Input (Double) Offset, (Double) Code, (Bool) SV or BPM, (Optional String) Extension
- Return NIL

**.Input_N_S:**

 - Initiates a SINGULAR note input prompt
 - Input (Optional Bool) Toggle Flooring Flag
 - Return (Double) Offset, (Int) Key Position

**.Input_N_M:**

 - Initiates a MULTIPLE note prompt
 - Input (Int) Number of Inputs, (Optional Bool) Toggle Flooring Flag
 - Return (VDouble) Offset, (VInt) Key Position

**.Input_T_S:**

 - Initiates a SINGULAR timing point prompt and returns a vector double
 - Input (Optional Bool) Toggle Flooring Flag
 - Return (Double) Offset, (Double) Code, (String) Extension

**.Input_T_M:**

 - Initiates a MULTIPLE timing point prompt and returns a vector double
 - Input (Int) Number of Inputs, (Optional Bool) Toggle Flooring Flag
 - Return (VDouble) Offset, (VDouble) Code, (VString) Extension

**.Flooring_S:**

 - Initiates the Flooring
 - Input (Double) Fix Offset
 - Return (Double) Fixed Offset

**.Flooring_M:**

 - Initiates the Flooring
 - Input (VDouble) Fix Offset List
 - Return (VDouble) Fixed Offset List

**.Input_Value_I:**

 - Initiates a integer prompt based on range and uses a loop to make sure a valid input is done
 - Input (Double) Lower Bound, (Double) Upper Bound, (Bool) Inclusive of End Points
 - Return (Int) User Input

**.Input_Value_D:**

 - Initiates a double prompt based on range and uses a loop to make sure a valid input is done
 - Input (Double) Lower Bound, (Double) Upper Bound, (Bool) Inclusive of End Points
 - Return (Double) User Input
