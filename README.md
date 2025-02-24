

# **CMOS-Based 3-bit Quad Computational Unit in LTSpice**  

## **Project Overview**  
This project implements a **3-bit computational unit** using **CMOS logic** in **LTSpice**. The design follows a **bottom-up approach**, starting from CMOS gates, combinational circuits, and integrating them into a **quad-computational unit**. The unit supports four operations:  
- **Addition (ADD)**  
- **Multiplication (MUL)**  
- **Greater Than (GT)**  
- **Arithmetic Shift Right (ASR)**  

A **decoder and multiplexer** are incorporated to control and select the required computational operation.  


## **Folder Structure**  

- [LT_Spice_Files](https://github.com/HanumanSagarBathula7392/Integrated_Computational_Circuit/tree/main/LTSPICE_FILES)  
    - SCHEMATIC.asc : For circuit schematic  
    - SYM.asy        : For Symbol representation  
    - TESTING.asc     : To Test circuit for validation  
    - PART_2_A_SYM.asc      : This is Overall design Schemating (PART_2_A_TESTING.asc for simulation) ((PART_2_A_SYM.asy for overall design symbol) 
    - [Project_Report.pdf](https://github.com/HanumanSagarBathula7392/Integrated_Computational_Circuit/blob/main/Project_Report.pdf) : Detailed explanation and results  


## **How to Open and Simulate the Design**  

1. **Open LTSpice** and navigate to the [LT_Spice_Files](https://github.com/HanumanSagarBathula7392/Integrated_Computational_Circuit/tree/main/LTSPICE_FILES) directory.  
2. **Load the main schematic**:  
   - Open `PART_2_A_SYM.asc` for the **circuit layout**.  
   - Open `PART_2_A_SYM.asy` to view the **custom symbol** for modularity.  
   - Open `PART_2_A_TESTING.asc` to verify the **functionality of the design**.  
3. **Run the Overall Design**:  
   - Open `PART_2A_TESTING.asc`.  
   - Ensure all necessary sub-files are present.  
   - Click **Run** to simulate the entire computational unit.  

## **Design Explanation**  
The computational unit is structured as follows:  

1. **Basic CMOS Logic Gates**  
   - Built from **PMOS and NMOS transistors**.  
   - Includes **AND, OR, NOT, XOR, XNOR**.  

2. **Combinational Circuit Blocks**  
   - **Half Adder & Full Adder** and then designed **Carry Select Adder** for addition.  
   - **Multiplier** designed using 2 two Carry Select Adders and Combinational Logic.  
   - **Comparator (GT operation)** to check A > B.  
   - **Arithmetic Shift Right (ASR)** for signed division or shifting.  

3. **Integration into the Computational Unit**  
   - Four **3-bit computation modules** are included using decoder and mutliplexer.  
   - A **2-to-4 decoder** activates one module at a time.  
   - A **4-to-1 multiplexer** selects the final output.  

4. **Control Mechanism**  
   - **Decoder inputs (DRin, DCin)** select the active computational unit.  
   - **Operation Selector (OPSEL0, OPSEL1)** chooses the required operation.  
   - **Multiplexer Selector (SEL1, SEL0)** determines the final output.  


## **Simulation and Verification**  
- The project includes various **test circuits** to validate each module.  
- The final design is confirmed with **waveform outputs matching expected results**.  

**Note:** To simulate the overall design, you must download all the files provided in the [LT_Spice_Files.](https://github.com/HanumanSagarBathula7392/Integrated_Computational_Circuit/tree/main/LTSPICE_FILES)

## License

This project is open-source and available under the MIT License.

## Contact

For any inquiries or discussions, feel free to reach out via [GitHub Issues](https://github.com/HanumanSagarBathula7392/Integrated_Computational_Circuit/issues).


## **Conclusion**  
This CMOS-based computational unit successfully demonstrates the integration of **digital logic design principles** into a **functional LTSpice simulation**. The project can be extended further for **larger bit-widths** or **optimized power/performance**.  



