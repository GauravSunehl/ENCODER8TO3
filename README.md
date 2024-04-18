# ENCODER8TO3
# Aim:
To simulate and synthesis encoder using vivado.
# Apparatus Required:
Vivado Xilinx 14.7 Spartan 6 FPGA
# Procedure:
```
STEP 1: Start the vivado software and select the name and the project.
STEP 2: Select the device family, device, package and speed.
STEP 3: Select new source in the new project and select verilog module as the source type.
STEP 4: Type the file name and module name and click next and then finish button. Type the code and save it.
STEP 5: Select the run simulation and then run behavioural simulation in the source window and click the check syntax.
STEP 6: Click the simulation to stimulate the program and give the inputs and verify the outputs as per the truth table.
STEP 7: Compare the output with the truth table.
```
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/824226c8-c767-44b5-ab35-26fed65b195e)
# Truth Table
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/e228c14b-b814-40c8-92eb-748d48570c04)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/6fa5fe84-fe6f-472d-b9c0-e6dfa17413d3)
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/7d147e2a-ba03-4714-baee-17615c9c50c1)
# Verilog Code:
```
module encoder(d,a,b,c);
input[7:0]d;
output a,b,c;
or (a,d[4],d[5],d[6],d[7]);
or (b,d[2],d[3],d[6],d[7]);
or (c,d[1],d[3],d[5],d[7]);
endmodule
```
# Output:
![encoder hdl](https://github.com/GauravSunehl/ENCODER8TO3/assets/166976407/24ecb5c1-dc5b-4ac8-bc47-f96fe056184a)
# Result:
Thus the verilog program for encoder has been simulated and verified successfully.

