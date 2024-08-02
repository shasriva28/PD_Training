**DAY 1:**

1. Checked and understood the OpenLANE directory structure in detail. Also, checked the pdk variant that we are using which is sky130A (sky130_fd_sc_hd) and the .ref and .tech files inside it. We will be working on **sky130nm** process node.

   a. libs.ref --> contains files specific to the technology.
   
   b. libs.tech --> contains files specific to the tool.

    ![image](https://github.com/user-attachments/assets/e94d2f48-9ee3-4225-8b43-d5f9b520ffae)
    ![image](https://github.com/user-attachments/assets/8bb31373-9baa-4829-9248-c3ddcce53638)

2. Learned how to invoke the OpenLANE tool and imported all the packages required to run this flow.
    
    ![image](https://github.com/user-attachments/assets/1f7d1e41-20a0-41f3-871b-eea37fd73285)

3. Checked the different available designs and the design we would be running which is **picorv32a**.
  Our design (picorv32a) directory contains 3 main files:

    a. src --> source file (RTL verilog file and SDC would be present here)

    b. config.tcl --> configuration file

    b. pdk specific config file --> highest priority, any configuration mentioned here would get honored over the default values or values mentioned in config.tcl.
   
    ![image](https://github.com/user-attachments/assets/20260212-35d6-4396-9e1b-463a5fdb1c73)
    ![image](https://github.com/user-attachments/assets/66355d93-5fab-4f1f-b555-fd343f2d8bbc)

4. Set up the design before starting the flow that is design preparation before running synthesis.

   ![image](https://github.com/user-attachments/assets/5c4315d6-915a-45ee-b8a4-fcad08d4bb34)

5. New directory (runs) got created in our design (picorv32a) directory. Everything except tmp directory is empty as of now.

   New dir path: /home/vsduser/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs


    ![image](https://github.com/user-attachments/assets/14c2fc72-b7df-46e4-bc10-c61b0a571dbb)

6. Ran the synthesis flow using command run_synthesis in the console.

    ![image](https://github.com/user-attachments/assets/d01bf73e-ae81-4b90-994b-01c7ac299748)

7. **Task: Find the flop ratio.**

    Flop ratio = Number of D Flip Flop/ Total number of cells
   
    Flop ratio = 1613/14876 = 0.10842
   
    Flop ratio % = 10.842%

    ![image](https://github.com/user-attachments/assets/3086b0f5-7daa-4168-a2f5-f7876fab576d)

    ![image](https://github.com/user-attachments/assets/fbb97068-d74c-488e-af74-3fcb979feef6)

8. Checked the results and reports folders for synthesis. We can see the synthesized netlist present in the results and various reports were generated such as synthesis statistics report, sta report, etc.

    ![image](https://github.com/user-attachments/assets/0958b212-3420-413b-81cb-9d120d60f362)


**DAY 2:**

1. **Chip Floorplanning and Powerplanning**

   1. Define width and height of Core and Die:

      a. Take a netlist and convert the gates and flip-flops into physical dimensions (square/rectangular box).
      
      b. Remove all the wires and place all the gates and flipflops in a single plate (combining all of them into one physical dimension) to calculate the area occupied by the netlist on a Silicon Wafer.
      
      c. Silicon Wafer contains a lot of Dies inside it and inside each Die there is a Core region.
      
      d. A Core is the section of the chip where the fundamental logic of the design is placed.
      
      e. A Die, which consists of core, is a small semiconductor material specimen on which the fundamental circuit is fabricated.
      
      f. Place all the logical cells (from b) inside the core and calculate the utilization factor. If logical cells occupy the complete area of the core, the utilization factor would be 1 which is not the practical scenario.

         **Utilization factor = (Area occupied by Netlist/ Total area of the Core)**

         **Aspect ratio = (Height of Core)/ (Width of Core)**

         If the aspect ratio is 1, it signifies that the chip is square-shaped else rectangle.

         ![image](https://github.com/user-attachments/assets/5a7f9b64-6963-4351-99ad-7150410bc370)

   2. Define locations of Preplaced cells:

      a. Preplaced cells are the black boxes having some specific functionality that is implemented once separately and then can be instantiated multiple times.
      
      b. Preplaced cells are macros or IPs like memory, clock-gating cell, comparator, mux.
      
      c. The arrangement of these IPs in a chip is referred as floorplanning.
      
      d. These IPs/blocks have user-defined locations, and hence are placed in the chip before automated placement-and-routing, and are called as preplaced cells.
      
      e. Automated placement and routing tools place the remaining logical cells in the design onto the chip.

      f. Place the preplaced cells on the basis of design scenario or design background.

   3. Surround preplaced cells with decoupling capacitors.

      a. Decoupling capacitors are the huge capacitors that are completely filled with charge. Voltage across the decoupling capacitor is equivalent to the supply voltage. If power supply is 1V, decap will be charged till 1V.

      b. Decoupling capacitor is placed very near and parallel to the circuit.

      c. Everytime the circuit switches, it draws current from decap, whereas the RL network is used to replenish the charge into decap.

      d. As the name suggests, decoupling capacitor decouples the circuit from the main supply.
      
      e. So, with the help of decap, we have taken care of the local communication.

   5. Powerplanning

      a. Issue: Ground bounce and voltage droop issue because of one power supply.

      b. Solution: power planning --> multiple power supply through mesh kind of structure for VDD and VSS.

   6. Pin Placement and logical cell placement blockage.

      a. Clock ports are bigger than the data ports because clock drives all seq cells continuosly, basically they drives all the flops in the full chip. So, we need the least resistance path for the clocks.

      b. Logical cell placement blockage: we block the area between core and die to avoid placement of any logical cells in those areas by automated placement and routing tools because that area is reserve for the pin locations.

      

      

      


    


  

   





  
