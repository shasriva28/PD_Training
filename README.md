# Table of Content

<div class="toc">
	<ul>
    		<li><a href="#header-0"> DAY 1 </a></li>
      <ul>
        		<li><a href="#header-0-1"> OpenLANE directory structure </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-0-2"> Design preparation step </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-0-3"> Review files after design prep and run synthesis </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-0-4"> Review results and reports of Synthesis </a></li>
 		</ul>
	</ul>
</div>

<div class="toc">
	<ul>
    		<li><a href="#header-1"> DAY 2 </a></li>
      <ul>
        		<li><a href="#header-1-1"> Chip floorplanning [Theory] </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-1-2"> Chip floorplanning [Lab] </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-1-3"> Placement & Routing [Theory] </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-1-4"> Need for characterization </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-1-5"> Placement [Lab]  </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-1-6"> Cell Design Flow  </a></li>
 		</ul>
      <ul>
         <li><a href="#header-1-7"> General Timing characterization parameters </a></li>
	</ul>
</div>

<div class="toc">
	<ul>
    		<li><a href="#header-2"> DAY 3 </a></li>
      <ul>
        		<li><a href="#header-2-1"> Labs for CMOS inverter ngspice simulations </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-2-2"> Inception of Layout And CMOS fabrication process </a></li>
	      <ul>
        		<li><a href="#header-2-2-1"> Selecting a substrate </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-2"> Creating active region for transistors </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-3"> N-well and P-well formation </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-4"> Formation of 'gate' </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-5"> Lightly doped drain (LDD) formation  </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-6"> Source and Drain formation </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-7"> Steps to form contacts and interconnects (local) </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-8"> Higher level metal formation </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-2-9"> Lab introduction to Sky130 basic layers layout and LEF using inverter  </a></li>
 		</ul>
 		</ul>
      <ul>
        		<li><a href="#header-2-3"> Sky130 Tech File Labs </a></li>
	      <ul>
        		<li><a href="#header-2-3-1"> Lab steps to create final SPICE deck using Sky130 tech </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-3-2"> Lab steps to characterize inverter using Sky130 model files </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-3-3"> Lab introduction to Magic tool options and DRC rules </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-3-4"> Lab introduction to Sky130 pdk's and steps to download labs </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-3-5"> Lab introduction to Magic and steps to load Sky130 tech-rules </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-2-3-6"> Lab exercise to fix the poly.9 error in Sky130 tech file </a></li>
 		</ul>
 		</ul>
 </ul>
</div>

<div class="toc">
	<ul>
    		<li><a href="#header-3"> DAY 4 </a></li>
      <ul>
        		<li><a href="#header-3-1"> Timing modelling using delay tables </a></li>
	      <ul>
        		<li><a href="#header-3-1-1"> Lab steps to convert grid info to track info </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-1-2"> Lab steps to convert magic layout to std cell LEF </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-1-3"> Introduction to timing libs and steps to include new cell in synthesis </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-1-4"> Introduction to delay tables </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-1-5"> Delay table usage Part 1 </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-1-6"> Delay table usage Part 2 </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-1-7"> Lab steps to configure synthesis settings to fix slack and include vsdinv </a></li>
 		</ul>
 		</ul>
		<ul>
        		<li><a href="#header-3-2"> Timing analysis with ideal clock using openSTA </a></li>
	      <ul>
        		<li><a href="#header-3-2-1"> Setup timing analysis and introduction to flip-flop setup time  </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-2-2"> Introduction to clock jitter and uncertainty </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-2-3"> Lab steps to configure OpenSTA for post-synth timing analysis </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-2-4">  Lab steps to optimize synthesis to reduce setup violations </a></li>
 		</ul>
 		</ul>
		<ul>
        		<li><a href="#header-3-3"> Clock tree synthesis TritonCTS and signal integrity </a></li>
	      <ul>
        		<li><a href="#header-3-3-1"> Clock tree routing and buffering using H-Tree algorithm </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-3-2"> Crosstalk and clock net shielding </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-3-3"> Lab steps to run CTS using TritonCTS </a></li>
 		</ul>
 		</ul>
		<ul>
        		<li><a href="#header-3-4"> Timing analysis with real clocks using openTSA </a></li>
	      <ul>
        		<li><a href="#header-3-4-1"> Setup timing analysis using real clocks </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-4-2"> Hold timing analysis using real clocks </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-4-3">  Lab steps to analyze timing with real clocks using OpenSTA </a></li>
 		</ul>
			<ul>
        		<li><a href="#header-3-4-4"> Lab steps to execute OpenSTA with right timing libraries and CTS assignment </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-3-4-5">  Lab steps to observe impact of bigger CTS buffers on setup and hold timing </a></li>
 		</ul>
 		</ul>
	</ul>
</div>

<div class="toc">
	<ul>
    		<li><a href="#header-4"> DAY 5 </a></li>
      <ul>
        		<li><a href="#header-4-1"> Routing and Design Rule check (DRC) </a></li>
	      <ul>
        		<li><a href="#header-4-1-1"> Introduction to Maze routing - Lee's Algorithm </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-4-1-2"> Lee Algorithm conclusion </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-4-1-3"> Design Rule Check </a></li>
 		</ul>
 		</ul>
   <ul>
        		<li><a href="#header-4-2"> Power Distribution Network and Routing </a></li>
	      <ul>
        		<li><a href="#header-4-2-1"> Lab steps to build power distribution network </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-4-2-2"> Lab steps from power straps to std cell power </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-4-2-3"> Basics of global and detail routing and configure TritonRoute </a></li>
 		</ul>
 		</ul>
      
   <ul>
        		<li><a href="#header-4-3"> TritonRoute Features </a></li>
	      <ul>
        		<li><a href="#header-4-3-1"> TritonRoute feature 1 - Honors pre-processed route guides </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-4-3-2"> TritonRoute Feature2 & 3 - Inter-guide connectivity and intra- & inter-layer routing </a></li>
 		</ul>
	      <ul>
        		<li><a href="#header-4-3-3"> TritonRoute method to handle connectivity </a></li>
 		</ul>
	   <ul>
        		<li><a href="#header-4-3-4"> Routing topology algorithm and final files list post-route </a></li>
 		</ul>
 		</ul>
 </ul>
</div>



# <h1 id="header-0"> DAY 1 </h1>
# <h2 id="header-0-1"> OpenLANE directory structure  </h2>

1. Checked and understood the OpenLANE directory structure in detail. Also, checked the pdk variant that we are using which is sky130A (sky130_fd_sc_hd) and the .ref and .tech files inside it. We will be working on **sky130nm** process node.

   a. libs.ref --> contains files specific to the technology.
   
   b. libs.tech --> contains files specific to the tool.

    ![image](https://github.com/user-attachments/assets/e94d2f48-9ee3-4225-8b43-d5f9b520ffae)
    ![image](https://github.com/user-attachments/assets/8bb31373-9baa-4829-9248-c3ddcce53638)

# <h2 id="header-0-2"> Design preparation step </h2>

3. Learned how to invoke the OpenLANE tool and imported all the packages required to run this flow.
    
    ![image](https://github.com/user-attachments/assets/1f7d1e41-20a0-41f3-871b-eea37fd73285)

# <h2 id="header-0-3"> Review files after design prep and run synthesis </h2>

5. Checked the different available designs and the design we would be running which is **picorv32a**.
  Our design (picorv32a) directory contains 3 main files:

    a. src --> source file (RTL verilog file and SDC would be present here)

    b. config.tcl --> configuration file

    b. pdk specific config file --> highest priority, any configuration mentioned here would get honored over the default values or values mentioned in config.tcl.
   
    ![image](https://github.com/user-attachments/assets/20260212-35d6-4396-9e1b-463a5fdb1c73)
    ![image](https://github.com/user-attachments/assets/66355d93-5fab-4f1f-b555-fd343f2d8bbc)

6. Set up the design before starting the flow that is design preparation before running synthesis.

   ![image](https://github.com/user-attachments/assets/5c4315d6-915a-45ee-b8a4-fcad08d4bb34)

7. New directory (runs) got created in our design (picorv32a) directory. Everything except tmp directory is empty as of now.

   New dir path: /home/vsduser/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs


    ![image](https://github.com/user-attachments/assets/14c2fc72-b7df-46e4-bc10-c61b0a571dbb)

8. Ran the synthesis flow using command run_synthesis in the console.

    ![image](https://github.com/user-attachments/assets/d01bf73e-ae81-4b90-994b-01c7ac299748)

9. **Task: Find the flop ratio.**

    Flop ratio = Number of D Flip Flop/ Total number of cells
   
    Flop ratio = 1613/14876 = 0.10842
   
    Flop ratio % = 10.842%

    ![image](https://github.com/user-attachments/assets/3086b0f5-7daa-4168-a2f5-f7876fab576d)

    ![image](https://github.com/user-attachments/assets/fbb97068-d74c-488e-af74-3fcb979feef6)

# <h2 id="header-0-4"> Review results and reports of Synthesis </h2>

11. Checked the results and reports folders for synthesis. We can see the synthesized netlist present in the results and various reports were generated such as synthesis statistics report, sta report, etc.

    ![image](https://github.com/user-attachments/assets/0958b212-3420-413b-81cb-9d120d60f362)


# <h1 id="header-1"> DAY 2 </h1>

# <h2 id="header-1-1">  Chip floorplanning [Theory] </h2>

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


# <h2 id="header-1-2">  Chip floorplanning [Lab] </h2>

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

# <h2 id="header-1-3"> Placement & Routing [Theory] </h2>

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

   FF1,1,2 and FF2 logics are abutted means there is no time delay between signal passed from FF1 to FF2. There are multiple reasons to do abutment, let's say this particular section of the circuit works at a very high speed and zero time delay is required, and don't want to waste delays on wires, and therefore, the abutment is done for those logics.

   So, now the complete logic has been optimized based on the placement condition.

   ![image](https://github.com/user-attachments/assets/bf6e972f-2fbd-48ed-9cc8-44c65338057f)


   Next, what we have to do is we have to check whether whatever we have done is correct or not. For that since the clocks have not built yet, we have to just check the data path over here considering there are no clocks or clocks are ideal.

   By ideal clock, we mean that the time required for a clock to reach any of the flip flops is zero.

# <h2 id="header-1-4"> Need for characterization </h2>

1. Typical IC design flow that every design needs to go through if it wants to be implemented onto a chip. So, the first step to do that is logic synthesis. If we have a functionality that is coded in the form of RTL, the first step is to convert the functionality into legal hardware is refer to as **logic synthesis.**

   So, the output of logic synthesis is nothing but an arrangement of gates that will represent your original functionality that you've described using an RTL. This is the first step of an IC design flow.

      ![image](https://github.com/user-attachments/assets/da60f97c-5f9f-4ae8-8f9c-de337c464a71)

2. The next step after logic synthesis is floorplanning. In this step, we import the output of logic synthesis or the netlist that we get out of the logic synthesis and decide the size of the core and die. So the size of the core and die is completely dependent on the amount of gates and the shapes and sizes of the gates present in the output of the logic synthesis.
   
3. After floorplanning, the placement stage is there, and then CTS (Clock Tree Synthesis). And then finally we have the routing stage.

      ![image](https://github.com/user-attachments/assets/d67148cd-cc1a-4a52-abcc-426a6eadd8e1)

     One thing is common across all the stages --> Gates or cells. Therefore, library characterization is very important and why this is so important.

     This collection of gates if you place it in some area, that area is referred to as Library.

     ![image](https://github.com/user-attachments/assets/3874c14f-e07b-4e40-aad2-13f4ebc9db60)

# <h2 id="header-1-5"> Placement [Lab] </h2>

1. We are doing a congestion-related placement, we are right now not considering the timing. We are just ensuring that the congestion is less.

2. There were 3 settings for placement. Placement in Openlane occurs in 2 stages: Global placement and detail placement.

   So, there are different tools to do both of these functionality.

   **Global placement** --> coarse placement, no legalization happening

   **What is legalization?** --> The standard cells are placed in standard cell rows, they should be exactly inside the row abutted with each other. And there should be no overlaps. Legalization is more required from a timing point of view.
   
   **Detail placement** --> legalization happens here

3. When we do **run_placement**, first global placement happens. Global placement, the main objective is reducing the wire length. In Openlane, we use the concept of HPWL means half-perimeter wire length. Reduction of HPWL is the main focus and converging the overflow (OVFL) means a decrease in the OVFL value means the placement is going right.

4. So, previously I had done till floorplan, for running the placement from the previous day's floorplan in Openlane, no need to run synthesis and floorplan again.

   Just do the following steps:

   a. package require openlane 0.9

   b. prep - design <design_name> -tag <desired_tag> --> ex: prep - design picorv32A -tag 08-08_11-13

   c. **run_placement**

      ![image](https://github.com/user-attachments/assets/d2c44e8e-07ef-47aa-8a04-b5bf867919fb)


5. Now, for opening the layout from the def file created through placement, use the same command as used for floorplan def, just replace the floorplan def with placement def.

      ![image](https://github.com/user-attachments/assets/cdca67bb-8a22-48ee-897e-96204d984fd2)

      ![image](https://github.com/user-attachments/assets/32330926-75ac-4b41-ab44-6d8db42823f6)

6. Zoomed in and checked the standard cells have been placed in standard cells rows.

   ![image](https://github.com/user-attachments/assets/8298e7a0-2e55-4bd0-a956-0aab2b21a229)

**Note: Power Distribution Network gets created during floorplan but in Openlane flow right now, the order is a little different. The floorplan does not create the Power Distribution Network. Here, in Openlane flow, PDN is done post floorplan, placement, and CTS.**

# <h2 id="header-1-6"> Cell Design Flow </h2>

 1. So, we have a placed and routed design here.
      
    Standard cells are placed in a section called Library. Library is a place where you keep all your standard cells, macros, IPs, decaps, etc.
    
    ![image](https://github.com/user-attachments/assets/1eeec68b-26a9-48c8-b9e0-0155f7426335)

    Library has got cells with different functionalities, different sizes, and different threshold voltages (Vt).

    ![image](https://github.com/user-attachments/assets/4f539a31-c6c0-48bd-a504-3aefad25684d)

2. The next step is to take one of the inverters and understand its cell design flow. This inverter has to be represented in the form of its shape, in the form of its timing behavior, in the form of its drive strength, and in the form of its power characteristics, and so on. A small inverter has to go through a typical cell design flow.

      Cell design flow is divided into 3 parts:

      ![image](https://github.com/user-attachments/assets/bd1b7c55-6d53-421f-9565-f72477c04730)

      1. **Inputs**: inputs to design your inverter, Process design kits (pdks) provided by the foundry.
   
         a. **DRC & LVS rules**: tech file --> has 5he rules like poly width, extension over active, etc.

            ![image](https://github.com/user-attachments/assets/f0547965-31bb-43e1-9f7d-abae19ffd10c)

         b. **SPICE models**:

            ![image](https://github.com/user-attachments/assets/11482134-a868-4ea3-ba73-80f8dbf35235)

         c. **Library & user-defined specs**: Cell-height, supply voltage, metal layers, pin location, drawn gate length, et
         

      2. **Design steps**:

         a. **Circuit design**: implement the function and model nmos and pmos to meet the library requirement, will get the information about W/L of the nmos and pmos in this step. Once we know the value of W/L for the transistors, next step is to implement these values in the layout called as layout design. Output of the Circuit design step is **CDL (circuit description language)**

            ![image](https://github.com/user-attachments/assets/68c9c05c-a50a-4a16-86b9-820fe840bb35)

         b. **Layout design**: First step is to get the function implemented through the mos transistors. The next step is to get the pmos network graph and nmos network graph. Output of the layout design - **GDSII, LEF, extracted spice netlist/ckt**

            ![image](https://github.com/user-attachments/assets/3fc02d34-353d-4217-9c5f-68621738190a)

            Next step is to obtain the Euler's path.

            ![image](https://github.com/user-attachments/assets/38db7e0d-7c17-4931-a3ba-270d63936432)

            Once you obtain a Euler's path, draw a stick diagram out of it.

            ![image](https://github.com/user-attachments/assets/6be57ed4-186b-48ea-98fa-d2c0ce0153e1)

            Next step is to convert this stick diagram into a proper/typical layout according to the rules from the inputs.

            Next step is to extract the parasitics and characterize them in terms of timing.

         c. **Characterization**:

            ![image](https://github.com/user-attachments/assets/5234cacf-713e-4362-9ac2-92875b5a37e1)

            So, what we have till this step:  layout of buffer, description of buffer, extracted spice netlist, subckts,  nmos pmos spice models, etc.

            ![image](https://github.com/user-attachments/assets/b6d2886c-d99f-4e49-9377-ee39c6ecdcd1)

            ![image](https://github.com/user-attachments/assets/df1aec31-4d71-4a5d-bff4-20242aaac85d)

      3. **Outputs**: these are actually used by the EDA tools.
  

# <h2 id="header-1-7"> General Timing characterization parameters </h2>

1. **Timing Characterization**:

      ![image](https://github.com/user-attachments/assets/e431c74b-78a9-4b7c-9cc3-8794e4a79db5)

      a. **Timing threshold desinitions**:

      ![image](https://github.com/user-attachments/assets/3804265a-eeca-4d9d-85e0-e3a1763ddd08)

      b. **Propagation delay**:

      ![image](https://github.com/user-attachments/assets/c5b7442a-c240-43fe-a457-672302b99d4b)

      c. **Transition time**:

      ![image](https://github.com/user-attachments/assets/02f94740-63f8-456d-90cf-72ee61ff931c)

      ![image](https://github.com/user-attachments/assets/cba5b2bf-4cac-4f41-a6db-8c2e5dfa5ccf)

      d. **Output current waveforrm**


# <h1 id="header-2"> DAY 3 </h1>

# <h2 id="header-2-1"> Labs for CMOS inverter ngspice simulations </h2>

1. In Openlane, we can do the **changes on the fly**. If suppose, we have already done the floorplan and observed a lot of congestion, we can change utilization factor even now. In our case, we have placed the IO pins equidistant, now we will be changing it to some other input output pin strategy. There are **4 strategies supported by the IO placer**.

   **IO placer is one of the open source EDA tool** which we used to place the IOs around the core.

   a. So now check the file where this mode for IO placement is set, first checked the README.md (under **openlane/configuration** dir) where lot of switches are defined but didn't find IO mode settings so now checked the floorplan.tcl (under **openlane/configuration** dir). It is set to 1 as shown in the below image.

   ![image](https://github.com/user-attachments/assets/50129e37-7e69-4deb-856d-9b633f15c767)

   b. We are setting it to 2 on the fly and then running floorplan again.

   ![image](https://github.com/user-attachments/assets/55288752-127b-49f4-9704-ee1a65156bbe)

   c. Again opened the layout in Magic and the def is updated (in the same folder only where previous def was there) and the IO pin placement is changed.

   ![image](https://github.com/user-attachments/assets/ac843b6b-254d-4ac1-82ce-db98a9d2383e)

   ![image](https://github.com/user-attachments/assets/c8832005-5798-4098-abb4-98906279235d)


2. **SPICE simulations**: 350nm, 250nm mos are available.

   1. Create a SPICE deck for **VTC CMOS** characteristics --> netlist 

      a. When we say W/L of mos it means it is the W/L of the channel of mos.

      b. In cmos, generally pmos should be wider than the nmos. **Ideally, pmos should be twice or thrice of the nmos.** But the spice deck we are creating is having nmos and pmos of the same W/L.

      ![image](https://github.com/user-attachments/assets/95a38834-1418-4fcb-b0bb-f49d67186991)

      M1 --> pmos, M2 --> nmos

      **Syntax of Mosfet in the SPICE: M1 Drain Gate Source Substrate type W L**

      ![image](https://github.com/user-attachments/assets/a5ca78d2-c533-45e0-92d6-cab4e9b72f0c)

      ![image](https://github.com/user-attachments/assets/e5d8dfc6-e0ba-480d-8ac6-b39516f21f10)

   2. SPICE simulation in ngspice:

      Wn, Wp --> nomos and pmos channel width

      Ln, Lp --> nmos and pmos channel length
  
      **Wn/Ln = Wp/Lp = 1.5**

      ![image](https://github.com/user-attachments/assets/5e0de600-54dc-4b49-972d-5f18d45d0e2f)

      **The above VTC is shifted towards the left from the centre. Why??**

   3. Now, we have increased the pmos width to 0.9375 (**2.5 times of nmos channel width**) --> pmos is bigger than nmos here

      **Wn/Ln = 1.5, Wp/Lp = 3.75**

      ![image](https://github.com/user-attachments/assets/8c9abcd6-346f-45c0-a42d-de8e2727d7f2)

      Now **the VTC is at the centre itself.**

   4. Analysis of the 2 VTCs obtained in previous 2 points (2 & 3).

      Shape of both the waveforms are similar --> means CMOS is a robust device, when input is low, ouput is high and vice-versa and this is for kinds of CMOS. Therefore, Cmos logic is even and **widely used for any of the logic gate designing**.

      What defines the robustness of the CMOS?

      1. **Switching threshold, Vm** --> point where Vin=Vout

         ![image](https://github.com/user-attachments/assets/ffb1a149-deec-43a6-b0f1-428481329cf0)

         This brings us to many conclusion here:

         1. This area is very critical area for CMOS inverter bcoz input=output.

         2. Both pmos and nmos are in saturation region in this area means both are kind of turned on that implies very high chance of leakage current. Direct current flow from power to ground means short ckt current.

         3. Here, Vin = Vout, means Gate voltage = Drain voltage which means Vgs >> threshold voltage.

            ![image](https://github.com/user-attachments/assets/bd8a5f7b-7fe1-4f1f-9cf2-fbee3d2b5403)

         4. Derivation of Vm: we are trying to proof robustness of switching threshold and trying to understand how does the switching threshold varies with varying pmos and nmos.
        
            ![image](https://github.com/user-attachments/assets/6748d31d-a839-491b-81b7-ebf5bc146dd0)


            1. We will also do **transient analysis** here and calculate the rise and fall delay. We will plot Vin and Vout with time on x-axis.

               Dynamic simulation SPICE netlist:

               ![image](https://github.com/user-attachments/assets/0aaaeda3-05c1-47c8-b00c-4b660057bd4f)

               ![image](https://github.com/user-attachments/assets/bec66b34-ea0c-4c70-ab92-de1163f517fc)

               Rise and fall delays are calculated using the above waveform. Basically, we see at what times input and output 50% rise/fall happening and then subtract the two. 

               Ex: **Rise delay = Time at Vout(50%) rise - time at Vin(50%) rise**

            2. So, we have done both static and dynamic simulation for the 1st case when Wn/Ln = Wp/Lp and got the Vm from the VTC where it cuts the 45 degree line.
           
               ![image](https://github.com/user-attachments/assets/62901b4d-aa12-4eea-980b-63eee968a197)

               
3. **Lab steps to git clone vsdstdcelldesign**

     1.  We will git clone one of the repositories that is custom made for this workshop.

         Git repository link: https://github.com/nickson-jose/vsdstdcelldesign

         **How to git clone**?

         Click on the green Code button and then copy the URL.

         ![image](https://github.com/user-attachments/assets/0792188e-23cb-447a-b2a8-7ffa6aaf0f2e)

         Now use **git clone** command in the terminal and paste the link.

         ![image](https://github.com/user-attachments/assets/074d1661-413c-4699-a352-854381a52973)

         A new folder **vsdstdcelldesign** got created in openlane dir.

         ![image](https://github.com/user-attachments/assets/61f5a8f6-aef4-41f8-a250-d5885d246c6e)

         ![image](https://github.com/user-attachments/assets/fa8c82e6-6882-4d94-92b1-fa2fc3169a33)

   2. Now, we will open the mag file and see the different layers that are used in the building of the inverter.

         Copy the tech file to this vsdstdcell design dir itself as we will be frequently using it.
   
         ![image](https://github.com/user-attachments/assets/e8ee555d-f797-4e77-a64b-49407a3b6204)

         ![image](https://github.com/user-attachments/assets/df661033-92a6-4b21-b6e0-aa7c9e57624c)

      	The read line that we are seeing in the above inverter layout is the polysilicon.

   
# <h2 id="header-2-2"> Inception of Layout And CMOS fabrication process </h2>

## 16-mask CMOS process

# <h3 id="header-2-2-1"> 1. Selecting a substrate </h3>

   Substrate is something on which you fabricate your complete design.

   There are various kind of substrate available but we will go for the most common one which we use for most of the mobile devices or any kind of device or chip you see in the real time --> **p-type**

   ![image](https://github.com/user-attachments/assets/0aa527d2-be4e-4c68-bd9b-67d6b690f93d)

# <h3 id="header-2-2-2"> 2. Creating active region for transistors </h3>

   1. Grow 40nm Silicon dioxide (SiO2) [act as an insulator] on the p-type substrate.

   2. Deposit a layer of 80nm Si3N4 over it.

   3. Deposit a layer of photoresist (1um) on top of it. Photoresist is a film, positive or negative film that see for old cameras. On this photoresist we are going to do some process.

   4. Mask1 --> When we talk about layouts those are nothing but mask in fabrication term. We basically protect some desired area through masking. In the below snippet that red color is masking. If there is UV light, then the area underneath those red masks are protected while the other resions are exposed to those UV light. So, we basically wash those resist area those are directly exposed to the UV light.

![image](https://github.com/user-attachments/assets/68b59a7f-4359-4831-9bbe-6d895dca5a50)
  
   5. After washing the exposed photoresist region:

![image](https://github.com/user-attachments/assets/63f98756-3a53-48c8-8273-ead08c04227a)

   6. Next step is to remove the mask: (These all are process of photolithography)

![image](https://github.com/user-attachments/assets/1405c7e8-f7a0-4b16-8e8e-f5d395f9a48d)

   7. Etched off the Si3N4, Only the area underneath the photoresist will be protected, the remaing Si3N4 area will be etched off.

![image](https://github.com/user-attachments/assets/847260b1-9685-4e07-a50c-1b90cd6db079)

   8. Next step is to remove the photoresist itself because Si3N4 itself will act as a very good protection layer to grow the oxides on the other area.

![image](https://github.com/user-attachments/assets/ea887a0d-cf51-47f0-badc-084acf164aef)

   9. Now we will put this complete thing into an oxidation furnace. A furnace is a place which works at very high temperature upto 900-1000 degree celsius that helps to grow the oxide in the other areas. We have grown the first layer of SiO2 in oxidation furnace itself. Now there will be second level of growth of oxidation.

![image](https://github.com/user-attachments/assets/32597180-4dff-40b2-8b1f-61750bd5e4ed)

	These areas of thick deposition of Si3N4 are called as isolation region and the **transistors at both the side won't be able to communicate to each other because of this isolation region**. This process that we have done is referred to as **LOCOS.**

![image](https://github.com/user-attachments/assets/aec1ffd4-4ab5-4b30-af15-b50c922915cf)

   10. Next step is to remove or etch oyt the Si3N4.

![image](https://github.com/user-attachments/assets/5899aacd-c163-401b-996a-17b2c2aa724b)

   11. So, we have got the **2 active regions where we actually grow transistors** and the isolation region will protect transistors so that they are not communicating with each other. So, we have actually created an **electrical isolation** over here.

# <h3 id="header-2-2-3"> 3. N-well and P-well formation  </h3>

   **N-well is used for pmos fabrication and P-well is used for nmos fabrication**. Both can't be done at the same time. We need to protect the one area while we fabricate the other.

   The same steps will be done here also, deposit a layer of photoresist then define pattren of layer you want to protect. So we are using Mask2 to protect one area first.

   ![image](https://github.com/user-attachments/assets/7769effc-6a34-422e-84b4-c01214650cb2)

   How does this Mask2 looks into the layout, lets see a top view of CMOS inverter in Magic.

   ![image](https://github.com/user-attachments/assets/eeb91356-3a63-4d63-b46f-329c2776205d)

   The right one is CMOS inverter and the left one is showing the Mask2 in the layout.

   Next step is to expose this photoresist to the UV light. So, same this UV light will react only to the exposed photoresist area.

   ![image](https://github.com/user-attachments/assets/e64ca778-f9be-4716-a5b2-0f2489bbe2b7)

   When we wash this particular thing into a solution, that exposed area of photoresist will washed away.

   ![image](https://github.com/user-attachments/assets/58baac40-94a5-4ad8-9bd5-a2ac6296192f)

   Now, the right area is available for any chemical reactions or anything we have to do over here.

   Next step is to remove the Mask2 also. And finally we have to create a **p-well** over here.

   P-well is created using Boron. Boron is a p-type material and it is diffused into this particular p-type substrate using a process called as **Ion implantation**. So, Boron being a p-type creates a P-well over here and the energy that is needed to diffuse the Boron through the oxide layer present is about 200keV.

   ![image](https://github.com/user-attachments/assets/70f5da1e-fc9d-4c7d-973b-856449d79c15)

   We will do the similar steps of the **N-well creation** also.

   ![image](https://github.com/user-attachments/assets/9bd5d112-bb73-46aa-b49a-0f09da3733ef)

   For N-well creation, we will use **Phosphorous** that is an n-type material and a bit heavier than Boron. Then again the Ion implantation of Phosphorous will be done to create the N-well.

   ![image](https://github.com/user-attachments/assets/fcd22667-2e1d-431b-8155-230a1ea6cbfc)

   ![image](https://github.com/user-attachments/assets/0a495508-a5f7-4b94-9527-7580d1dd5f7c)

   So, we have created the wells over here but the depths of the wells are not finalized yet. So, this was just the well creation.

   Next we have to diffuse the wells so that it occupies almost half of the substrate area. So that we have a clear room available for pmos and nmos fabrication.

   So, the next step is to take this thing, this complete substrate into a high temperature furnace. It is called as **Drive in furnace**.

   Push it to a very high temp for a very long time about 11 degree celcius for 4-5 hrs.

   So, this will diffuse the Boro and Phosphorous atoms into the p-type substrate forming the clear wells. This is called as **Twin tub process.**

   In N-well, we are going to create pmos transistor and in P-well, we are going to create nmos transistor.

   ![image](https://github.com/user-attachments/assets/c4efcec4-d0a9-4fbb-a842-be2d5ce8871b)

# <h3 id="header-2-2-4"> 4. Formation of 'gate' </h3>

   ![image](https://github.com/user-attachments/assets/5d45c934-713f-42d9-a8ec-bc20a1cbb156)

   ![image](https://github.com/user-attachments/assets/9ef42721-dbb4-4808-a6b7-2b5a12ea2672)

   We are going to control the oxide capacitance and the doping concentration through the further steps.

   So the next step for the formation of gate is to control the doping concentration.

   Same masking steps again, repetetive steps.

   **Threshold Voltage controlling:**

   ![image](https://github.com/user-attachments/assets/3ae10306-48cf-4546-a899-6e6871667167)

   ![image](https://github.com/user-attachments/assets/936a2108-554e-419f-8766-2eac93895317)

   ![image](https://github.com/user-attachments/assets/2933ba62-40e8-4124-9b9a-9defe21d43c9)

   ![image](https://github.com/user-attachments/assets/b69c62f8-5ed7-4206-b7d3-c91815f638b4)

   **Fixing of oxide:** --> that got damaged while Ion implantations.

   ![image](https://github.com/user-attachments/assets/4d15488f-3cfc-40c1-8102-b2da31ccd0d1)

   ![image](https://github.com/user-attachments/assets/d02cb341-3707-4cff-a31a-55a3f6f386ec)

   Now the **formation of gate** step:

   ![image](https://github.com/user-attachments/assets/bcc47194-673b-4f3c-9513-2b25f97a70ee)

   ![image](https://github.com/user-attachments/assets/62744e7a-3c3d-439f-8004-1e916f7f54e1)

   ![image](https://github.com/user-attachments/assets/be715c8f-b0c5-488f-b91d-2565ef063127)

   ![image](https://github.com/user-attachments/assets/3d083492-98ef-4056-97c3-59a7250a8f6c)

   ![image](https://github.com/user-attachments/assets/ae966f7f-93cc-4c89-a651-7970966a3ea2)

   ![image](https://github.com/user-attachments/assets/5f44a829-0bf9-49ae-8752-55269d6f2f13)

   ![image](https://github.com/user-attachments/assets/70ba1725-0c13-418a-b0e3-caa8db0a915a)

# <h3 id="header-2-2-5"> 5. Lightly doped drain (LDD) formation </h3>

   What we want to achieve over here is the doping profile that is **P+,P-,N in N-well where we are trying to fabricate the PMOS**.

   Similarly, for the **NMOS that is being fabricated in the P-well**, we need **N+,N-,P **doping profile.

   ![image](https://github.com/user-attachments/assets/48fccbe5-4ef9-44a7-b64f-2aa9eea0ef05)

   **Why do we need these kind of doping profiles?**

   1. Hot electron effect:

		![image](https://github.com/user-attachments/assets/71d4de63-158f-43e4-901a-ee4c51916d16)

   2. Short channel effect:

		![image](https://github.com/user-attachments/assets/0b78b2c0-bbad-4b17-bf0f-476f7293895f)


   ![image](https://github.com/user-attachments/assets/cc357fa6-0946-40d5-872f-c85aacb03604)

   ![image](https://github.com/user-attachments/assets/07ee560b-3d77-4049-b321-c905c618f5ea)

   ![image](https://github.com/user-attachments/assets/1dd03dc8-1390-452c-827b-020782f66ae3)

   ![image](https://github.com/user-attachments/assets/76e29f5e-ac49-430e-95d8-c80330005aae)

   **How to protect from further Source and Drain formation?**

   ![image](https://github.com/user-attachments/assets/93090819-44a2-4c83-9709-3bd0c7bc96ae)

   ![image](https://github.com/user-attachments/assets/a28b7dcc-8956-4b0f-97d9-40eeb61f5877)

   ![image](https://github.com/user-attachments/assets/d69aac7a-c49a-410a-81ff-1ad53e8072c8)

   ![image](https://github.com/user-attachments/assets/9664121c-97ed-4bf0-9487-73745d63df27)

# <h3 id="header-2-2-6"> 6. Source and Drain formation </h3>

   The next step is to add a **thin layer of screen oxide** to avoid the effect of channeling.

   Channeling is an effect when you do a lot of ion implantation, if the vector velocity of our ions match with that of the crystaline structure of the p-type substrate, the ions might go deep inside the p-type substrate without even hitting any of the silicon atoms.

   ![image](https://github.com/user-attachments/assets/1a77e5fb-ab33-4969-bbbb-8fc0688add3f)

   ![image](https://github.com/user-attachments/assets/c92cd386-e783-443b-b0be-e0a05f62f497)

   ![image](https://github.com/user-attachments/assets/7bb738cc-858d-4799-a557-42dca97e4ca4)

   ![image](https://github.com/user-attachments/assets/36c05222-67a8-4667-85f3-d7c51cdec4bd)

   ![image](https://github.com/user-attachments/assets/a9317ab5-9154-47d6-badb-e6fb542376eb)

   ![image](https://github.com/user-attachments/assets/f19a0d29-c207-49e4-a4c5-32d4ee922c7b)

   ![image](https://github.com/user-attachments/assets/0fc00b73-49a6-4387-92a0-972a24d03a67)

   So, we will put this half built pmos and nmos to high temperature furnace.

   ![image](https://github.com/user-attachments/assets/87048080-6f8d-4661-8105-c8c52c627172)

# <h3 id="header-2-2-7"> 7. Steps to form contacts and interconnects (local) </h3>

   Contacts are really very imp because thats the only thing that is accessible to an user through which you can control the electrical characteristics of pmos and nmos.

   ![image](https://github.com/user-attachments/assets/232fc1fd-3bf0-4c4e-9f35-5e0ff5d0e703)

   ![image](https://github.com/user-attachments/assets/18783ae3-4c9d-4d53-a756-2e3a1f66291d)

   ![image](https://github.com/user-attachments/assets/a1cb4afc-c770-4f36-ba06-95d327bb007e)

   ![image](https://github.com/user-attachments/assets/d22c75f2-446a-4b49-a175-29d3212cfdc2)

   ![image](https://github.com/user-attachments/assets/f07d62c9-1edf-49c4-b771-ac0b3009fca1)

   ![image](https://github.com/user-attachments/assets/70c6d039-5bcc-4444-8772-c3a37d8836c2)

   ![image](https://github.com/user-attachments/assets/7e04045c-d2dd-41fa-b768-ac0812cafac6)

   ![image](https://github.com/user-attachments/assets/01de4957-986a-4f85-a441-204f5f2ca5e7)

   ![image](https://github.com/user-attachments/assets/88a475c9-825a-473d-8646-92fc28c0a01c)

   ![image](https://github.com/user-attachments/assets/05baa5ad-bd03-4663-b6f3-62b1bf3ea218)

   ![image](https://github.com/user-attachments/assets/7b08776c-93d3-4900-8e07-9fe39e33b5e7)

   ![image](https://github.com/user-attachments/assets/0c1e05cf-7712-4e9a-a1ee-0e918ba141bf)


# <h3 id="header-2-2-8"> 8. Higher level metal formation </h3>

   One thing to notice here is that we have non planar surface topography and its not a good idea to deposit the metal interconnects on this layer. There are some problems wrt metal discontinuity.
   
   So, we need to planerious this surface.

   ![image](https://github.com/user-attachments/assets/004e0659-e5ca-4ce5-a9c4-317a82a30b44)

   ![image](https://github.com/user-attachments/assets/c0fae799-4765-4d29-ac28-c1d4e0195379)

   ![image](https://github.com/user-attachments/assets/fb9a7732-5e3f-4d6d-9e16-3c305b10163a)

   ![image](https://github.com/user-attachments/assets/d65f6ec4-949e-4636-a7e8-fd68ae5b1c0f)

   ![image](https://github.com/user-attachments/assets/d2fbb614-89a2-4c12-91e7-d3c5918db197)

   ![image](https://github.com/user-attachments/assets/d8df0306-a66c-47ca-a411-507bf0dfc835)

   ![image](https://github.com/user-attachments/assets/d3f693dc-728b-4938-b272-480c438596fd)

   ![image](https://github.com/user-attachments/assets/12503801-a485-4adb-851a-52693f4d317b)

   ![image](https://github.com/user-attachments/assets/9fd4023b-bc83-43c4-bed6-49ae5e15b49d)

   ![image](https://github.com/user-attachments/assets/281eec81-4990-4301-ad20-eb9e66886f9f)

   ![image](https://github.com/user-attachments/assets/1a20b5a3-1ab5-484f-a043-508f7580f00c)

   ![image](https://github.com/user-attachments/assets/98f0c330-8c40-4386-a3fe-f82ad4a536af)

   Till here, we have the **local interconnects (0 level of metal), 1st level of interconnects (Aluminium interconnects)**.

   Now the next step is to again take this **metal levels to the higher level metal**.

   ![image](https://github.com/user-attachments/assets/43416f56-f290-4abc-a307-28ccfdf8c027)

   ![image](https://github.com/user-attachments/assets/3ac165de-2668-46c0-886b-5bc593fb5e98)

   ![image](https://github.com/user-attachments/assets/02fc3279-0195-4297-af64-5b14250fd7e8)

   **TiN acts an additional layer to SiO2 and acts as the barrier between lower and higher metal layers**.

   ![image](https://github.com/user-attachments/assets/6586fa91-4e71-4cf8-85e6-19c13afb89e2)

   ![image](https://github.com/user-attachments/assets/112c38cc-8b98-4082-b1a6-250480c812be)

   ![image](https://github.com/user-attachments/assets/af3ed65d-3751-419c-97ce-7fcb2c08f654)

   ![image](https://github.com/user-attachments/assets/16620b28-a6e4-4dc9-94c1-41d63797c3eb)

   **So, this is how 16 mask CMOS process will look like:**

   ![image](https://github.com/user-attachments/assets/c5033982-833d-410e-9984-44ef950a8ec6)


# <h3 id="header-2-2-9"> 9. Lab introduction to Sky130 basic layers layout and LEF using inverter </h3>

1. On the right side of the CMOS inverter layout, we have all color palets, these are basically the layers.

   ![image](https://github.com/user-attachments/assets/87b8ec98-1cf1-4b14-9f7c-5b6c4de3af3d)

   Green is the ndifusion layer, for verifying you can go to the green color in the color palet and it will show ndiffusion written at the top right bar.

   **When the poly crosses n-diffusion, its an NMOS. Similarly, when the poly crosses p-diffusion, its a PMOS.**

   For verifying the NMOS, we selected the region and then wrote what in the tkcon, it came out to be NMOS.

   ![image](https://github.com/user-attachments/assets/8dbeeaca-11d2-4a33-b0da-ebed992874f0)

   Similarly, we did for PMOS.

   ![image](https://github.com/user-attachments/assets/6b032002-2362-4053-83d7-f5773ab20a75)

   Now we will verify that the drain of PMOS and NMOS are connected.

   For that, **place your cursor at the output pin Y and press S twice**, all the highlighed boundary in white in connected which shows that drains of both PMOS & NMOS are connected.

   ![image](https://github.com/user-attachments/assets/45892997-b290-474e-ab62-5efb0080d3f6)

   Now, check the connection of source of PMOS:

   ![image](https://github.com/user-attachments/assets/04450162-3bb4-4f87-a79f-8a559e7a052e)

   So, source of the PMOS is connected to VDD net.

   Similarly, verified that the source of NMOS is connected to ground.

   ![image](https://github.com/user-attachments/assets/d43d0d19-082d-44a4-8ab1-c01ff7354524)

   **Lab steps to create std cell layout and extract spice netlist:** https://github.com/nickson-jose/vsdstdcelldesign

   How do we know what is the logical function of this inverter?

   For that, **we would first extract this SPICE and post that we will do simulations in ngspice.**

   **To extract it on spice:**

   Open the tkcon window and see where we are and extract it in a file using the **command extract all.**

   ![image](https://github.com/user-attachments/assets/066d70b3-0518-42aa-acaa-6be95d93d99b)

   ![image](https://github.com/user-attachments/assets/ce0473f0-bc40-49f0-ae7a-b3479e2b394b)

   Now, we will use this ext file to create spice file to be used with the ngspice tool using command **ext2spice**.

   ![image](https://github.com/user-attachments/assets/78f73d30-08aa-4eb8-8b7c-4e23b79ae13c)

   ![image](https://github.com/user-attachments/assets/4169dcae-69a1-4c2f-9d1e-a50e74cafed8)

   **Extracted spice netlist:**

   ![image](https://github.com/user-attachments/assets/f4ec0899-2ca6-474f-b564-1d30c2d8662d)


# <h2 id="header-2-3"> Sky130 Tech File Labs </h2>

# <h3 id="header-2-3-1"> 1. Lab steps to create final SPICE deck using Sky130 tech </h3>

1. Netlist:

	Doubel tick ones are defined in the netlist. We need to add some more lines to SPICE code for the below circuit.

 	![image](https://github.com/user-attachments/assets/b503b8bc-1d21-44a5-ad89-076a5f78096f)

2. Edited SPICE netlist:

	![image](https://github.com/user-attachments/assets/179696c9-d58d-456a-99de-7fc728a7940e)

 	We will run it in ngspice and will check the result.

	![image](https://github.com/user-attachments/assets/522922c5-dc0c-4e65-badd-4900372a81bb)

	Plotted the Y vs time A

	![image](https://github.com/user-attachments/assets/77cc4283-a90e-4d9d-bc10-eaf1b75b8184)

	![image](https://github.com/user-attachments/assets/8744ce53-d655-4597-935e-06f5f0472bf0)


	We can see the spikes, load is very less, will modify the netlist.

	Edited netlist:

	![image](https://github.com/user-attachments/assets/aabaa437-d355-4f9b-b58d-40a6386ea032)

	![image](https://github.com/user-attachments/assets/3d76c55b-8ef4-415e-900b-7ecca46fb7b3)

	![image](https://github.com/user-attachments/assets/18a213e6-9238-489e-a010-5110018dc7dd)


# <h3 id="header-2-3-2"> 2. Lab steps to characterize inverter using Sky130 model files </h3>

1. Rise Transition --> Time taken by the output to rise from 20 to 80% of the max value.

	20% of 3.3 = 0.66, 80% of 3.3 = 2.64

   	![image](https://github.com/user-attachments/assets/1930236d-6c57-4f0a-8805-e69a334d7a93)

   	**Rise transition = 0.064 ns**

 	Similarly, **Fall transition = 0.042 ns**

2. Cell Fall/Rise delay --> cell propagation delay when the output is falling/rising between 50% of the values.

	50% of 3.3 V = 1.65 V

	So we will fine the time diff between input and output when the value is 1.65 V.

	![image](https://github.com/user-attachments/assets/e6d45d96-a4f2-4612-b7c4-c0b9c0123679)

	**rise delay = 0.061 ns**

   	Similarly, **fall delay = 0.027 ns**

   So, we have got all the four parameters above, the **cell characterization is done.**

# <h3 id="header-2-3-3"> 3. Lab introduction to Magic tool options and DRC rules </h3>

![image](https://github.com/user-attachments/assets/a402f4ab-afb1-402a-a7c8-66dc467c8626)

![image](https://github.com/user-attachments/assets/bd8442e1-c742-401f-bfc2-c7e0630fd7ba)

**Magic DRC documentation**: http://opencircuitdesign.com/magic/


# <h3 id="header-2-3-4"> 4. Lab introduction to Sky130 pdk's and steps to download labs </h3>

![image](https://github.com/user-attachments/assets/d194228c-54da-4093-b480-6b9e364acf98)

**Skywater documentation**: https://skywater-pdk.readthedocs.io/en/main/rules/background.html

**DRC rules**: http://opencircuitdesign.com/magic/techref/maint2.html#drc

![image](https://github.com/user-attachments/assets/309a86cc-4911-4fd4-8322-0b2b138ae4ec)

![image](https://github.com/user-attachments/assets/78228bf6-69ad-4df3-b63d-6fde571393f0)

![image](https://github.com/user-attachments/assets/5393599d-fb06-444f-9adc-241a6bdcf182)

![image](https://github.com/user-attachments/assets/d4d832ad-574c-47b5-9249-660e238ff1fe)


# <h3 id="header-2-3-5"> 5. Lab introduction to Magic and steps to load Sky130 tech-rules </h3>

![image](https://github.com/user-attachments/assets/cc0b4c43-8f06-48d6-a985-1c3929433248)

![image](https://github.com/user-attachments/assets/9cf3aef2-e65a-425a-be3a-f199467341a5)

![image](https://github.com/user-attachments/assets/9ed92dff-17d1-48ae-a476-175a18d82de3)

**Rules mentioned in Skywater pdk:**

![image](https://github.com/user-attachments/assets/6e82adf1-b7d6-4360-b8ea-a39ae0a224ee)

Creating m3 contact: make a box with left click and right click like we select an object and then hover over m3 contact in color plate and **press pk.**

![image](https://github.com/user-attachments/assets/803c14bc-c438-424e-a730-5b09575d2df7)

type : to go to the tkcon shell and type **cif see VIA2** to see the contact cuts.

![image](https://github.com/user-attachments/assets/52bdb5f8-2466-4be0-a4b5-cb86c81ccf99)

![image](https://github.com/user-attachments/assets/b7b76d4c-db72-48e3-9ad4-de7091c8c408)


# <h3 id="header-2-3-6"> 6. Lab exercise to fix the poly.9 error in Sky130 tech file </h3>

![image](https://github.com/user-attachments/assets/0ab9ef23-8d03-4ad7-aba8-3db9317972e3)

![image](https://github.com/user-attachments/assets/d329fd2d-848d-4744-872f-01c185609836)

![image](https://github.com/user-attachments/assets/0c9df517-eb1d-4a26-9970-59c2a2840e17)

Before editing:

![image](https://github.com/user-attachments/assets/f2841315-1eb1-48ef-9885-5b7768f61a39)

After editing:

![image](https://github.com/user-attachments/assets/64af4348-b4fa-4f27-8754-e741c51ecfef)

Now search for aliases:

![image](https://github.com/user-attachments/assets/9c7f758a-d83a-4acf-89e5-1a34313b0094)

![image](https://github.com/user-attachments/assets/3619fc17-7b33-4305-95cf-2942b4e8aef6)

![image](https://github.com/user-attachments/assets/ad48e28a-a604-40d5-9ed1-60249bc99c5e)

![image](https://github.com/user-attachments/assets/cbe5d27b-d118-4bbe-ad9b-175d674bf330)


# <h1 id="header-3"> DAY 4 </h1>

# <h2 id="header-3-1"> Timing modelling using delay tables </h2>

# <h3 id="header-3-1-1"> 1. Lab steps to convert grid info to track info </h3>

First step would be to extract a LEF file out of this sky130_inv.mag file.

Open the tracks.info file: [ Tracks are used in the routing stage]

![image](https://github.com/user-attachments/assets/7ce732bb-0157-4cdb-bf65-5234f8091271)

**Press G** to activate the grid in Magic.

**Input and Output ports should be at the intersection of horizontal and vertical tracks.** --> This is the 1st requirement.

![image](https://github.com/user-attachments/assets/b42bdb85-63b8-4145-9519-b607234eae06)

Grid boxes have taken the dimension that we have provided:

![image](https://github.com/user-attachments/assets/77c7cc61-af86-4b72-af7d-18bba7a83ab8)

So, we have converted the grid according to the track info.

# <h3 id="header-3-1-2"> 2. Lab steps to convert magic layout to std cell LEF </h3>

The 2nd requirement is that the width of the std cells should be in the odd multiples of the x pitch of that layer.

We have verified that the layout of the inverter is as per the requirements of the PNR tool.

Creation of port example:

![image](https://github.com/user-attachments/assets/6bd2f4e9-61e9-497a-a263-f9f6116303d6)

Now we are ready to extract the LEF file from this .mag.

Saved used a custom name sky130_shasriva.mag.

![image](https://github.com/user-attachments/assets/92bfd8ae-dc5d-4069-af64-45fdbc1444ba)

![image](https://github.com/user-attachments/assets/798f8e22-cbb9-4f30-bf48-aa96853bd94d)

Open the new custom .mag file and do **lef write**.

![image](https://github.com/user-attachments/assets/a9aa6b08-4d68-4c56-935b-5f70c2044c4b)

![image](https://github.com/user-attachments/assets/4ff53237-1217-4cbf-8f05-6f2057c5d80e)

![image](https://github.com/user-attachments/assets/326c1a93-dc7b-4db8-9ec4-61a0c6019dee)

# <h3 id="header-3-1-3"> 3. Introduction to timing libs and steps to include new cell in synthesis </h3>

**Basic idea is to include the custom cell in the OpenLANE flow.**

Copy the custom lef files and the libs in this src dir:

![image](https://github.com/user-attachments/assets/aee751fa-5cd6-4410-9c88-d03b1c3c825d)

![image](https://github.com/user-attachments/assets/2c61943d-4266-40c6-8253-cc9414e0b633)

Now we need to modify our config.tcl.

Original config.tcl:

![image](https://github.com/user-attachments/assets/d9627bcb-9450-4a52-b481-e5d061c472d8)

Modified Config.tcl:

![image](https://github.com/user-attachments/assets/3bc19a04-38b7-436e-85d4-965930c1d432)

![image](https://github.com/user-attachments/assets/c1486f7e-727e-4fa9-aa0d-b54f03037391)

![image](https://github.com/user-attachments/assets/41937b10-be1f-49bb-9efa-fd48fc997865)

![image](https://github.com/user-attachments/assets/f758a53f-4e9b-4fca-aba8-80f98159ad3a)

# <h3 id="header-3-1-4"> 4. Introduction to delay tables </h3>

![image](https://github.com/user-attachments/assets/6277f445-c720-44e5-8e30-833eca09ebb9)

The advantage of using above circuits in the clock tree is that the rest of the circuit for the amount of time CLK is not getting propagated through the gates, there will be no switching and short ckt power that will be consumed by the clock tree during that period of time.
So, lot of power is getting save during that time.

Using these kind of AND and OR gates in clock tree is basically known as **clock gating**.

Can we blindly swipe any buffer in the clock tree to such AND/OR gate as shown in the below snippet?

![image](https://github.com/user-attachments/assets/6fb4f65a-6aa4-4aae-903d-1ca0d1cd83ba)

![image](https://github.com/user-attachments/assets/dc2e86fa-3129-4f53-bccb-2cd07dea7977)

Why are we doing this particular observation as in the above snippet? Why do we even need this kind of observation?

The Cload at the output of the buffers at each level will not be same for the whole clock tree.

If load is varying, input transition will also vary for buffers at each level.

So, we have varying input transition and varying output load for any buffer.

So, problem here is that we will have the variety of delays. How to capture that?

The solution is **Delay tables.** and the delay tables become the **Timing model** of a particular buffer of a particular size, vt (threshold voltage).

![image](https://github.com/user-attachments/assets/3ec3c878-5899-4c87-b339-457b7c399ffc)

# <h3 id="header-3-1-5"> 5. Delay table usage Part 1 </h3>

CBUF'1' = Clock buffer of size 1.

![image](https://github.com/user-attachments/assets/ee09f76d-f18d-44fc-985d-755f718b1f25)

Example with some real values:

Those delay values whose values are not present in the table, those are **extrapolated based on the given data in the table**.

![image](https://github.com/user-attachments/assets/6dc2d86d-5183-4a4d-8128-614d5d6c9408)

Lets say the delay for **CBUF'1' came out to be x9'** [some value between x9 and x10 obtained after extrapolation].


# <h3 id="header-3-1-6"> 6. Delay table usage Part 2 </h3>

![image](https://github.com/user-attachments/assets/31725b3f-ef4b-4d59-9229-e99b15ffb0de)

Now, we need to calculate the **latency** from the input of buffer 1 to the point it is reaching the input of the flip-flops.

Let us ignore the wire delay for now.

For all the 4 paths to the flip flop, **the delay/latency is x9'+y15**. 

So the **skew at any of the four inputs to flip flops is 0**.

![image](https://github.com/user-attachments/assets/3b72c4e3-f897-4dd9-89e4-c6dd3d6facd9)

If at every level, each node won't be driving the same load, then we would have got a **non-zero skew value.** That's why, it is always preferred that each node driving the same load at every level.

**Power aware CTS**: For some time frame, some flops are not active, or are active only under certain conditions. So that section of the chip has got some special functionality that will turn on only under certain conditions. So, in that case we need to propagate the clock tree and stop it at 2 itself. That is how **we can obtain a Power Aware Clock Tree.**

![image](https://github.com/user-attachments/assets/67bebaf4-3208-46c9-a37d-9dafb782a17e)


# <h3 id="header-3-1-7"> 7. Lab steps to configure synthesis settings to fix slack and include vsdinv </h3>

![image](https://github.com/user-attachments/assets/d8dfb63a-e71c-4f7f-b4b5-34ee624b69a1)

**We are changing some of the switches and rerunning synthesis to see if we can get some reduced slack.**

![image](https://github.com/user-attachments/assets/94a030ed-c0ba-4922-8063-f45681b87f6f)

Slack din't change for my case while in the video it got reduced significantly.

![image](https://github.com/user-attachments/assets/82a72cbd-919a-4206-a851-745c0a338e1b)

**Tried again from the start from the design preparation stage:**

![image](https://github.com/user-attachments/assets/3cfb5885-56e2-4240-9cdc-29d2c485a91c)

![image](https://github.com/user-attachments/assets/0bbc8886-d01f-4301-a81d-265433f69d3b)

Now, **chip area got increased and tns and wns became 0**:

![image](https://github.com/user-attachments/assets/e69a59f9-6b34-41d3-a8b9-796ad027214d)

**Timing report is showing no paths found**.

![image](https://github.com/user-attachments/assets/b9efb7ac-7bef-4217-8581-78cf121e78e3)

Now, we will **run_floorplan:**

floorplan failed:

![image](https://github.com/user-attachments/assets/0deef31d-04d7-4c1d-96b1-7db2edadbbab)

Error shows that there are no macros in the design, so we should skip this macro step.

Instead of running run_floorplan cmd, we can break the cmd wrapper to its atomic cmds, which as per floorplan.tcl is as below:

init_floorplan

place_io

global_placement_or

tap_decap_or

![image](https://github.com/user-attachments/assets/9d373594-ecc3-49b7-b25b-5c8b2b1be9bf)

![image](https://github.com/user-attachments/assets/05c61180-7c54-488a-8568-99e5fa32c4e3)

![image](https://github.com/user-attachments/assets/b166ccb5-86b4-49ea-8314-ccb6fce222f3)

![image](https://github.com/user-attachments/assets/a0beafe1-f381-45ff-9845-03d8f3692414)

Also, checked the **merged.lef and our custom cell is present there**.

![image](https://github.com/user-attachments/assets/ae1ac620-aaad-40af-9516-abe5a0c783e6)

Now, we will **run_placement:**

![image](https://github.com/user-attachments/assets/44ca89d5-6fbf-4878-9ee2-893146005009)

Now, we will check our custom cell in the placement:

![image](https://github.com/user-attachments/assets/3470e03e-cb05-4fe3-93c2-54c42cdc25e0)

# <h2 id="header-3-2"> Timing analysis with ideal clock using openSTA </h2>

# <h3 id="header-3-2-1"> 1. Setup timing analysis and introduction to flip-flop setup time </h3>

![image](https://github.com/user-attachments/assets/bbdee146-d569-4d13-9c1b-4ac34ff562d0)

![image](https://github.com/user-attachments/assets/d400a883-bca1-4b0f-ae6c-2e51520c36db)

![image](https://github.com/user-attachments/assets/ff7e2b70-d371-4200-bcc5-80e940761b75)

![image](https://github.com/user-attachments/assets/a6fb3e00-a177-4ece-b5db-f8161522c551)

![image](https://github.com/user-attachments/assets/5f95b04e-8943-469c-9c91-50d047d3d506)


# <h3 id="header-3-2-2"> 2. Introduction to clock jitter and uncertainty </h3>

![image](https://github.com/user-attachments/assets/24c259fe-ad93-4c89-bdc3-09b80c5c95f1)

![image](https://github.com/user-attachments/assets/0018d38b-7e00-44bf-b7a8-f6acf30d50bd)

![image](https://github.com/user-attachments/assets/7443cfcb-c459-4e29-a790-6901213134d9)

![image](https://github.com/user-attachments/assets/a7d2f720-dc41-4cdb-ba32-1da40ec0e063)

![image](https://github.com/user-attachments/assets/cbbbc293-b944-412e-b839-c240cba3ee5a)

So, we will identify the **logic with single clock** first in our design:

![image](https://github.com/user-attachments/assets/d1bf79f8-9e9f-46e4-836d-e8edfd780afb)

![image](https://github.com/user-attachments/assets/9f0df51e-055c-4075-806c-8d3a364436d1)

![image](https://github.com/user-attachments/assets/87eb8ef6-d04a-46de-8cba-3c676f234137)

![image](https://github.com/user-attachments/assets/4b442e09-20bb-4be5-808f-7334bd8ae74e)

# <h3 id="header-3-2-3"> 3. Lab steps to configure OpenSTA for post-synth timing analysis </h3>

Created pre_sta.conf file in openlane dir.

We have got zero tns and wns, therefore doing for verilog file in synthesis directory.

![image](https://github.com/user-attachments/assets/e66024f3-9da9-4894-945c-b07aff0f08f5)

![image](https://github.com/user-attachments/assets/65653d01-9075-4024-b7cb-1e9376942544)

![image](https://github.com/user-attachments/assets/c5b85fcd-1649-434f-ade7-2e070cef2f07)

Right now, hold time does not hold any significance because we have not done CTS. We are assuming ideal clocks that means skew is zero that means **Hold anaylsis will ve overly optimistic, so it will come into picture after CTS**.

So, lets check for the setup analysis.

# <h3 id="header-3-2-4"> 4. Lab steps to optimize synthesis to reduce setup violations </h3>

Lets upsize this buffer selected in the below snippet:

![image](https://github.com/user-attachments/assets/d5679797-b3d9-4241-ad6b-669e29e09e2f)

**This buffer is driver 4 input pins**:

![image](https://github.com/user-attachments/assets/f20c6d82-e83e-4a8d-b9d4-db8ab4bfd78e)

So we are replacing it with a bigger buffer (drive strength=4), it will cost more area but will check after replacing.

![image](https://github.com/user-attachments/assets/10934271-4c96-43da-b68b-a37bc4b240cb)

![image](https://github.com/user-attachments/assets/0785c7c8-2df0-436f-bfb0-b51670e79779)

So the **slack has reduced**:

![image](https://github.com/user-attachments/assets/0e1f656d-140c-496e-93e3-6a008770f63b)

**Path has changed, therefore we are checking for the previous report path:**

Current report path:

![image](https://github.com/user-attachments/assets/da08f769-7465-4ffb-b0d1-c39e9f9bed01)

Previous report path:

![image](https://github.com/user-attachments/assets/5477426d-624f-4690-8eea-4482d50dba5e)

![image](https://github.com/user-attachments/assets/e92726cf-0efc-466f-8c51-6c1ea2f812fe)

The **slack is met:**

![image](https://github.com/user-attachments/assets/2bd77a18-7c4c-4872-88f8-550817084aed)

![image](https://github.com/user-attachments/assets/62a0f419-0bf3-4fb7-9a71-75fc4110220d)

# <h2 id="header-3-3"> Clock tree synthesis TritonCTS and signal integrity </h2>

# <h3 id="header-3-3-1"> Clock tree routing and buffering using H-Tree algorithm </h3>

![image](https://github.com/user-attachments/assets/43d9b22b-4632-450a-b92e-60f1d444c289)

Lets blindly connect them:

![image](https://github.com/user-attachments/assets/b19f563e-e561-4ba6-891a-0eee40ffb53e)

Now lets see **what is the problem with this clock routes:**

![image](https://github.com/user-attachments/assets/a3f22275-a264-4d32-a3d8-b14fb2374158)

Skew should be close to 0 and the tree that we have build is not a good tree.

Now we will build a **H-tree that follows mid point strategy**. So, the skew will be close to 0.

![image](https://github.com/user-attachments/assets/fe563d8c-7501-4783-b0af-1dcd85ad8144)

![image](https://github.com/user-attachments/assets/0791a5a3-0521-42a5-be66-5a95494b312f)

**Problem: signal integrity**

![image](https://github.com/user-attachments/assets/46772a75-35f5-4d06-8beb-71b6a9146311)

**Solution: Add repeaters** --> Repeaters used in the clock path have got **equal rise and fall** [Red buffers].

![image](https://github.com/user-attachments/assets/a7fe5790-38b1-4e8e-a446-d031a87ff68f)

# <h3 id="header-3-3-2"> Crosstalk and clock net shielding </h3>

![image](https://github.com/user-attachments/assets/6d3e7dd3-7a14-4eaf-bf00-9a0d07184635)

![image](https://github.com/user-attachments/assets/c712dba5-1cbe-4948-bfab-a04e851a164f)

![image](https://github.com/user-attachments/assets/a9c4cc19-7212-4ddf-aa0d-1b4ef91ba209)

![image](https://github.com/user-attachments/assets/57c9e870-e94f-4161-9108-f298f4436e76)

**How to shield?** -> Place a VDD and VSS wire parallel to signal wire.

# <h3 id="header-3-3-3"> Lab steps to run CTS using TritonCTS </h3>

Now, **we will replace the previous verilog netlist with this new slack corrected netlist**:

![image](https://github.com/user-attachments/assets/00184f0d-48ac-4771-93aa-e863cc3a3dcb)

Verified the new netlist by searching the buffer that we have made as buf_4:

![image](https://github.com/user-attachments/assets/72eafe99-32ee-4a7c-8ca1-2cf3b320ccf5)

Then we will **run_floorplan** and **run_placement** again and then **run_cts**.

![image](https://github.com/user-attachments/assets/1bb1a003-fd5a-42b6-9c09-e8bc24cdc781)

![image](https://github.com/user-attachments/assets/c3bb3505-1f93-491b-91cd-94e4664a97d0)

New verilog file created with CTS done - clock path & buffers

# <h2 id="header-3-4"> Timing analysis with real clocks using openSTA </h2>

# <h3 id="header-3-4-1"> Setup timing analysis using real clocks </h3>

**Setup Timing Analysis**:

![image](https://github.com/user-attachments/assets/834dd105-839a-4553-bfd1-2e728331375c)

![image](https://github.com/user-attachments/assets/6a43208e-9d00-4674-84a6-85cd28b6b143)

![image](https://github.com/user-attachments/assets/6e4afabc-7431-4382-a4f8-9f94c33e2a62)

![image](https://github.com/user-attachments/assets/fc1d7790-284d-430e-be9b-2fd1718829fd)

**If the slack is negative, we call it as violation**.

# <h3 id="header-3-4-2"> Hold timing analysis using real clocks </h3>

**Hold Timing Analysis**

![image](https://github.com/user-attachments/assets/59b85f46-8bdd-4b46-978b-8d8a715243b8)

![image](https://github.com/user-attachments/assets/d972e735-0eba-4576-bf7d-6595e13fc721)

![image](https://github.com/user-attachments/assets/b5c29222-fc03-413e-bde5-f0d86057bb38)

![image](https://github.com/user-attachments/assets/70d641f3-c198-43c1-a869-eb41ee4057c7)

Here, uncertainity dosen't play a role much because the same clock edge is going to both the flops so amount of jitter that will play a role for launch flop and the capture flop will be same.

![image](https://github.com/user-attachments/assets/eb64341d-c0e0-4615-85bb-b45da2ef0b3c)

**HU = Hold uncertainity**

![image](https://github.com/user-attachments/assets/ce1aee81-e1bf-4ff7-a0dd-4ec849257237)

![image](https://github.com/user-attachments/assets/437490c6-6d93-4602-b4ab-accaaf6a9558)

![image](https://github.com/user-attachments/assets/b78cd7fb-da90-4578-8c35-6198dbab7a8b)

![image](https://github.com/user-attachments/assets/0262e3be-dfb1-4aed-88bf-904cecc7a5c4)

![image](https://github.com/user-attachments/assets/9a1247d4-3057-408d-afc7-dc7809e73036)

# <h3 id="header-3-4-3"> Lab steps to analyze timing with real clocks using OpenSTA </h3>

Now our objective is to do the analysis of the clock tree of the entire ckt as the clock tree has been built.

Now we will invoke openroad in openlane itself instead of opening opensta separately for doing static timing analysis.

OpenSTA is already integrated in Openroad.

![image](https://github.com/user-attachments/assets/c7dc1c60-19d5-48a4-b57f-bb155b02d629)

Now we need to create a db. db is created from a lef and def file.

**read_lef**

![image](https://github.com/user-attachments/assets/8efdc1bc-cb27-4aa7-a8b1-7b026a6ea90b)

similarly, do **read_def** <def file after cts location (results/cts)>

Then, do **write_db <any_custom_name>**

ex: **write_db pico_cts.db**

![image](https://github.com/user-attachments/assets/bc204dee-14ca-4b0b-8bbb-69e2c55fdc29)

Verified that the **db got created in the openlane dir**.

Then **read_db**

![image](https://github.com/user-attachments/assets/9a95da74-57b9-40f6-84e7-f029055b51b8)

Now the clocks have been built, **we can calculate the actual cell delay in the clock path using set_propagated_clock**.

![image](https://github.com/user-attachments/assets/dc3c88db-e03e-46aa-8d16-cd197fc7c186)

![image](https://github.com/user-attachments/assets/0b92e582-cc76-4eb8-9d38-e8667c5ff09f)

![image](https://github.com/user-attachments/assets/45537bc1-1086-45f0-85c6-c07eb457f489)

# <h3 id="header-3-4-4"> Lab steps to execute OpenSTA with right timing libraries and CTS assignment </h3>

Now, type exit to exit from the openroad but you will still be in openlane.

Exploring Post CTS analysis by removing clkbuf_1 from clock buffer list variable.

![image](https://github.com/user-attachments/assets/9be904b1-483b-4933-b226-72a0955f61da)

Tool always picks buffers left to right as buf 2 is greater in area than buf 1.

![image](https://github.com/user-attachments/assets/eb123ea7-b8bd-4a56-b245-cd3b6d534a37)

![image](https://github.com/user-attachments/assets/5c69b5cc-e92b-4a9f-86e4-c48ff5c0b225)


# <h3 id="header-3-4-5"> Lab steps to observe impact of bigger CTS buffers on setup and hold timing </h3>

Now, we again need to create a db like we did earlier.

![image](https://github.com/user-attachments/assets/9739c8fc-7c9f-497e-969f-5b135303cf20)

![image](https://github.com/user-attachments/assets/d02a435a-896a-492d-a167-4d04db20e15e)

![image](https://github.com/user-attachments/assets/af40e0a8-2477-4e00-a38e-304612123e0e)

**Slack slightly improved at cost of area**.

![image](https://github.com/user-attachments/assets/b1557896-50bd-4cdd-bd96-a145e2b58ab2)

![image](https://github.com/user-attachments/assets/7395c666-982e-4540-a44b-77e1cc32b893)

![image](https://github.com/user-attachments/assets/59eede28-4e9f-483a-9e4d-8a196d30dc64)

# <h1 id="header-4"> DAY 5 </h1>

# <h2 id="header-4-1">  Routing and Design Rule check (DRC) </h2>

# <h3 id="header-4-1-1"> Introduction to Maze routing - Lee's Algorithm </h3>

![image](https://github.com/user-attachments/assets/d72bc88c-76ab-4c78-9680-4e9e134772a0)

When we say routing, means we need to connect 2 points with the best possible path, shortest possible path with less number of zig-zag lines, most of them should be L-shaped, there should be few with z-shaped and very few zig-zag lines.

![image](https://github.com/user-attachments/assets/af367be4-bd87-40b9-98dc-c2fd24659804)

**Lee's algorithm:**

First the **routing grid** will be created at the backend.

And the two points get created those are Source (S) and Target (T):

Algorithm labels the abjacent grids around S (Source). First adjacent grids are labelled as 1 and then around 1 as 2, then around 2 as 3 and so on till it reaches T (Target).

![image](https://github.com/user-attachments/assets/57038041-6870-4c47-9d31-30cbe087b563)

# <h3 id="header-4-1-2"> Lee Algorithm conclusion </h3>

![image](https://github.com/user-attachments/assets/c30524da-7e5b-49f4-a8ed-194f92ce0714)

Multiple paths are possible based on the numbering, we have to select the most optimum path.

![image](https://github.com/user-attachments/assets/05d39d3b-8ed5-49de-828d-71f27afcad79)

**Two bends** are there in the above path.

![image](https://github.com/user-attachments/assets/9952c483-2fd1-4caa-8882-1932a062ad58)

**Single bend** is there in the above path. So, this path will be preferred for routing S and T.

Limitations of Lee's algorithm:

1. Consumes a lot of time because lot of information needs to be stored.

2. Consumes huge memory.



# <h3 id="header-4-1-3"> Design Rule Check </h3>

There are some rules to do a proper routing and those are called as Design Rule Check (DRC).

![image](https://github.com/user-attachments/assets/68f4cdb6-a678-40c6-b4a1-1e00c3269ea8)

![image](https://github.com/user-attachments/assets/390ad14d-1151-4caa-bb65-e27fe0b90329)

![image](https://github.com/user-attachments/assets/18ae733b-9cba-41e6-8aa8-0b63c3722033)

![image](https://github.com/user-attachments/assets/ac395bcd-afd8-4c64-ae93-bceec643f9cc)

How to solve this issue of signal shorts?

Use different layers for routing of those 2 wires:

![image](https://github.com/user-attachments/assets/c730cb17-918d-4dc3-ab54-7a9bba6cb1b7)

![image](https://github.com/user-attachments/assets/2fb8e6b6-8185-4440-935e-bf0b00690d08)

![image](https://github.com/user-attachments/assets/90dc91f9-25bb-4a99-85cf-fe13eff2207b)

![image](https://github.com/user-attachments/assets/10ef1b99-bee9-4b1c-9c4b-0190492b7539)

**Parasitics extraction:**

![image](https://github.com/user-attachments/assets/a2ccc8ec-b205-4cfd-ad62-31b4603d0176)


# <h2 id="header-4-2"> Power Distribution Network and Routing  </h2>

# <h3 id="header-4-2-1"> Lab steps to build power distribution network </h3>

![image](https://github.com/user-attachments/assets/d50ba99b-528a-4370-8bce-3e740ad66975)

**How to know which was the last stage we ran in the flow?**

use command **echo $::env(CURRENT_DEF)** --> it will give you the location of last stage DEF that is CTS def.

To run pdn, type **gen_pdn**.

![image](https://github.com/user-attachments/assets/90b5f1af-c462-4d0f-93fb-67da2c566427)

![image](https://github.com/user-attachments/assets/c7027d21-c897-4737-8b6e-8d2a826012ce)

![image](https://github.com/user-attachments/assets/e85b018f-ed77-4d56-bd93-5d5b1512ec0c)

![image](https://github.com/user-attachments/assets/27c6e7ba-480a-4f47-bbb3-9cc69c62c5f8)


# <h3 id="header-4-2-2"> Lab steps from power straps to std cell power </h3>

![image](https://github.com/user-attachments/assets/0c7b6385-c1a7-46b5-9fc5-d3906dc4c980)

![image](https://github.com/user-attachments/assets/7cc62c64-ae16-4785-affc-2c18e6ea1dd3)


# <h3 id="header-4-2-3"> Basics of global and detail routing and configure TritonRoute </h3>

**Switches available for routing:**

![image](https://github.com/user-attachments/assets/0ec04dae-b1c3-41a2-92c5-cc65ef0f0dc3)

![image](https://github.com/user-attachments/assets/5cf5a704-2e33-4101-80dd-36cf7394b423)

Now, **run_routing**:

![image](https://github.com/user-attachments/assets/09d93b9a-c282-45f7-9803-8fb15b679f8a)

![image](https://github.com/user-attachments/assets/11708e19-c38b-4c3c-8c0a-c2e045a5a0cc)

Number of violations = 0

![image](https://github.com/user-attachments/assets/0b41c1fb-9e4e-4aa8-af40-a9165a46b216)

Routing Using **TritonRoute**:

![image](https://github.com/user-attachments/assets/e2beccf9-81cf-4f5a-9519-a4fc73a1593c)

![image](https://github.com/user-attachments/assets/4d8a6aa4-f133-42d9-b1d5-16c2a9391727)


# <h2 id="header-4-3"> TritonRoute Features  </h2>

# <h3 id="header-4-3-1"> TritonRoute feature 1 - Honors pre-processed route guides </h3>

![image](https://github.com/user-attachments/assets/c4ff3dfd-87bc-4c36-a5ec-d63b02dd82a2)

Intra-layer means within the layer.

Inter - layer means in between the layers.

**Route guides are something that we obtain after global route using Fast route engine.**

Output of the Fast route is Routing guide.

![image](https://github.com/user-attachments/assets/b8a456a5-9545-4ea2-8fac-d651b5f59371)

# <h3 id="header-4-3-2"> TritonRoute Feature2 & 3 - Inter-guide connectivity and intra- & inter-layer routing </h3>

![image](https://github.com/user-attachments/assets/c245e906-1b4c-402d-a5f1-b74b3be31985)

![image](https://github.com/user-attachments/assets/ba3d1e26-aada-4ad1-bd2c-082db149a9fc)

**Dashed line in the below snippet is panel.**

![image](https://github.com/user-attachments/assets/8ddd4124-d501-401f-981c-d17c32221198)

First routing in M1 is done (will be greyed out) and then routing in M2 is done and M3 and then so on. This is **sequential routing**.

![image](https://github.com/user-attachments/assets/52c1ee3d-1117-4a29-bce8-f4b2b378e15f)

# <h3 id="header-4-3-3"> TritonRoute method to handle connectivity </h3>

**TritonRoute --> when the detailed route is happened, below are the inputs:**

![image](https://github.com/user-attachments/assets/1cc7c813-1ec6-4ba8-87b9-5bb0e331d145)

![image](https://github.com/user-attachments/assets/0f4724d3-7956-4fdd-add1-52bbf705cce5)

![image](https://github.com/user-attachments/assets/ec61346b-5088-400c-816f-640b1f38df02)


# <h3 id="header-4-3-4"> Routing topology algorithm and final files list post-route </h3>

![image](https://github.com/user-attachments/assets/42e0c94a-315c-445b-bac6-9d48c7f52074)

![image](https://github.com/user-attachments/assets/b58e6f5c-340f-4e7a-b485-675ea2a92d4e)

![image](https://github.com/user-attachments/assets/0a9aeba3-bc7f-41a2-bf48-7ab2ed374a76)

![image](https://github.com/user-attachments/assets/43a6eec0-2baf-47be-8248-9ab68791316c)

![image](https://github.com/user-attachments/assets/258113f4-b888-49db-bf1a-a6873a1f054c)

![image](https://github.com/user-attachments/assets/5ee24713-a435-4298-b020-70e0f6fbfeb3)

![image](https://github.com/user-attachments/assets/63d52c05-b5ea-4615-b0ff-afe3d2beef23)

![image](https://github.com/user-attachments/assets/1369e76d-7370-4ff9-a8b5-af24f99f06fc)



























































































	












   

   
   



   







   

   

   

   


   








   

   

   
















   


   


   


   









	

   




   


   

   




   



   





   



   





   

   



   











   

   






   



   

	


 

   


      


               


            


         


      
      


      





      





         

         


         


         



   

     


      

   




   












      







      

      

      


    


  

   





  
