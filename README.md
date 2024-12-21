## NAME:MANIMARAN V
## REG.NO:24008541
## EXPERIMENT 5:ENCODER 8TO3 DATAFLOW MOEDLLING

## AIM:

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

## SOFTWARE REQUIRED: QUARTUS PRIME

## THEORY

## ENCODED 8 To 3

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

## TRUTH TABLE

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

## PROCEDURE

1. ## UNDERSTAND THE FUNCTIONALITY OF THE ENCODER  
   An 8-to-3 encoder has 8 input lines and 3 output lines. The output represents the binary index of the highest-priority input that is active (logic '1').

2. ## ASSIGN PRIORITY TO INPUTS
   Inputs with higher indices have higher priority (e.g., `D[7]` has the highest priority, `D[0]` the lowest).

3. ## DEFINE THE TRUTH TABLE
   Construct a truth table showing the binary output for each active input. If multiple inputs are active, the output corresponds to the highest-priority input.

4. ## FORMULATE BOOLEAN EXPRESSIONS  
   Derive expressions for each output (`Y[2]`, `Y[1]`, `Y[0]`) based on the truth table.

5. ## SET UP THE VERILOG MODULE
   - Define a module with 8 inputs (`D[7:0]`) and 3 outputs (`Y[2:0]`).
   - Use `assign` statements to describe the logic in the dataflow model.

6. ## IMPLEMENT THE LOGIC IN DATAFLOW MODELING 
   Write continuous assignment statements (`assign`) to implement the boolean equations for the outputs.

7. ## TEST THE DESIGN
   - Create a testbench to apply various input combinations.
   - Verify the outputs against the truth table.

8. ## SIMULATE AND DEBUG  
   - Use a simulation tool to validate the implementation.
   - Resolve any discrepancies or errors encountered during simulation.

## PROGRAM

![Screenshot 2024-12-21 170724](https://github.com/user-attachments/assets/74ed6cee-7231-402f-9bf3-47f7b7efe466)


## RTL LOGIC FOR ENCODED 8 To 3 IN DATAFLOW MODELLING
![Screenshot 2024-12-21 170735](https://github.com/user-attachments/assets/4cdb635b-e13b-4edf-9170-5a925b0dc545)

## TIMING DIGRAMS FOR ENCODED 8 To 3 in DATAFLOW MODELLING
![Screenshot 2024-12-21 170742](https://github.com/user-attachments/assets/c0f49730-6078-46f3-a25a-39c01727237d)

## RESULTS

Thus the Encoder 8 To 3 in Dataflow Modelling using verilog and validating
their functionality using their functional tables is implemented


