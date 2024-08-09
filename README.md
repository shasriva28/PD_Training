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

**Chip Floorplanning and Powerplanning**

   1. Define width and height of Core and Die:

      a. Take a netlist and convert the gates and flip-flops into physical dimensions (square/rectangular box).
         
         ![image](https://github.com/user-attachments/assets/17138d7b-9cc8-471a-b9e9-1d89f1ed52bb)

      b. Remove all the wires and place all the gates and flipflops in a single plate (combining all of them into one physical dimension) to calculate the area occupied by the netlist on a Silicon Wafer.

         ![image](https://github.com/user-attachments/assets/589005c7-a1b9-4efe-a1af-3444b0fb3920)
      
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


**   LAB**

1. In OpenLANE, we have a lot of switches (variables/options/settings) for each step (synthesis, floorplan, placement, etc) to adjust the flow that is present in README.md inside the configuration dir of OpenLANE.

   ![image](https://github.com/user-attachments/assets/7d03fe5a-3573-4135-8679-c91e6bfae84b)

   README.md:

   ![image](https://github.com/user-attachments/assets/63b691f9-dd6b-407e-91e3-8c1b39258b18)

   ![image](https://github.com/user-attachments/assets/fafe3e35-a038-41ff-b704-ebd1f7bdfe5e)

2. Where are the switches set?

   In the .tcl file of the specific stage, Ex: floorplan.tcl file in configuration dir is used for setting switches for floorplan.

   less floorplan.tcl

   ![image](https://github.com/user-attachments/assets/6e527b08-e6ce-4b34-a652-f5d090192a4f)

   floorplan.tcl has the lowest priority.

   priority order: floorplan.tcl < config.tcl (openlane/designs/picorv32a) < pdk specific config file (openlane/designs/picorv32a) [Day1, point3]

   In openlane flow, Horizontal metals (FP_IO_HMETAL) and Vertical metals (FP_IO_VMETAL) are 1 more than what is specified in the config file.

**Floorplan**

1. Ran the floorplan stage using command run_floorplan.

   ![image](https://github.com/user-attachments/assets/ec4889e9-a19a-4c26-98d5-de75a8ebc21a)

2. config.tcl inside the runs/latest_run will provide you the configuration taken by the flow. So, from this file, we can verify which config file switches got the highest priority.

      ![image](https://github.com/user-attachments/assets/3d514f4e-d223-4363-98c1-6f9ca3021517)

      We have verified the FP_CORE_UTIL and FP_IO_HMETAL, FP_IO_VMETAL from the 3 config files mentioned in point 2.
      
      1. FP_CORE_UTIL --> set as 50 in floorplan.tcl and 35 in sky130A_sky130A_fd_sc_hd_config.tcl (pdk specific config file).

         35 got the priority.
 
      3. FP_IO_HMETAL, FP_IO_VMETAL --> set as 4,3 in floorplan.tcl and 3,2 in config.tcl (openlane/designs/picorv32a)

         **Note: In this tool, whatever value we specify for HMETAL and VMETAL, +1 gets applied.**

         4,3 got applied means config.tcl (openlane/designs/picorv32a) got the higher priority.

          ![image](https://github.com/user-attachments/assets/79fd0a1a-eb22-484d-b781-7e01b2c712e6)

3. The floorplan stage is completed and we will look how floorplan looks like. First we will go the results/floorplan directory and we can observe the def (Design Exchange Format) file.

      ![image](https://github.com/user-attachments/assets/d7ca9362-f6b1-4a6e-ad53-91cdd4378dbf)

      ![image](https://github.com/user-attachments/assets/1ba81ddb-e933-488b-a4b8-ba738c64c65d)

      (0 0) --> (lower left x value, lower left y value)
         
      (660685 671405) --> (upper right x value, upper right y value)

      Unit is set by --> **UNITS DISTANCE MICRONS 1000** --> this is database unit per micron, i.e., 1 micron equals 1000 database units

      So **dividing these numbers (660685 671405) by 1000 will give the dimension of the chip in micrometer.**
   
4. To see the actual layout after the floorplan, we will use magic tool.
  
      To open the layout:

      ![image](https://github.com/user-attachments/assets/8954924d-8a54-47f9-a24f-f56a2cf1cd37)

      The layout was not in the center when we opened it. **To bring it in the center of the window**: press s on your keyboard to select the entire layout and then press v to fit it to the window.
  
      **For zooming into a particular portion of the layout** --> First do a left mouse click and then do a right mouse click to form a box and then press z on the keyboard.
  
      ![image](https://github.com/user-attachments/assets/d7b00427-84c6-4e12-92c2-a17da6e43df5)

      We had set the **input-output pin mode as 1 means setting the input-output pins equidistant** and we can see that the pins are equidistant in the layout.

      **For selecting any object** in the layout let's say a pin, just place your cursor over it and press s on your keyboard.

      Now, select a pin a see on which layer it is. So after selecting type **'what'** in the tkcon window.

      For a **horizontal pin, it came as metal 3** and for a **vertical pin, it came as metal 2** which was there in the config file.

      ![image](https://github.com/user-attachments/assets/6cccd79d-21b9-49f7-aa0b-8ff32354b84a)

      ![image](https://github.com/user-attachments/assets/f478b9cb-0c3e-4522-9c2d-1dc42d2076a1)

      ![image](https://github.com/user-attachments/assets/b122f73f-f655-471d-9040-40ecac0f9fdf)

      Tap cells are meant to avoid the latch-up condition that occurs in the CMOS devices. So, basically in the tap cell, nwell in connected to the VDD and the substrate to the ground to prevent latch-up.

5. Floorplan does not do the placement of standard cells but they are present in the lower left corner of the layout.

   ![image](https://github.com/user-attachments/assets/0e6563cb-f915-415d-a39d-d64d7a80280f)

**Placement & Routing**

1. Bind netlist with physical cells --> The netlist contains different gates and the shape of each gate defines its functionality, ex: by the shape of OR gate we understand that it will perform OR operation. But in reality, we don't have such shapes for different gates, we just have a box structure for each gate that has some width and height (physical dimension).

   ![image](https://github.com/user-attachments/assets/11919e8c-2d20-49c0-b883-4bd1ca639564)

   ![image](https://github.com/user-attachments/assets/e3cd10d7-ff20-4a5d-ab21-4034f67824d8)

2. Placement --> Once we have given proper shapes and sizes to each gate, the next step is to take those particular shapes and sizes and place them onto the floorplan.

      Till here, we have the floorplan, netlist, and physical view of the logic gates.

      ![image](https://github.com/user-attachments/assets/c5815070-6e67-4179-98a2-a21e91d5274e)

      Now we will do the placement of the standard cells in the floorplan.

      ![image](https://github.com/user-attachments/assets/8a9dbc6c-de14-4ac7-918c-24d31a5ffb05)

3. Optimize placement --> This is the stage where we estimate wire length and capacitance and, based on that, insert repeaters.

   Repeaters are buffers that will recondition the original signal, make a new signal that replicates the original signal, and send it again.

   So, signal integrity is maintained using repeaters but there is a loss of area. More repeaters means more area occupied by the repeaters on the floorplan but we have to live with it since we have to maintain the signal integrity.

   **Note: Slew depends on the value of the capacitor, the higher the value of the capacitor --> the amount of charge required to charge the capacitor will be high and the slew will be even bad.**

   ![image](https://github.com/user-attachments/assets/3cc4af3a-08e8-40f7-bac9-3c50aa9cc3df)

   
   












      







      

      

      


    


  

   





  
