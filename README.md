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
 		</ul>
      <ul>
        		<li><a href="#header-2-3">  </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-2-4">  </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-2-5">   </a></li>
 		</ul>
      <ul>
        		<li><a href="#header-2-6">   </a></li>
 		</ul>
      <ul>
         <li><a href="#header-2-7">  </a></li>
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

   
# <h2 id="header-2-2"> Inception of Layout And CMOS fabrication process </h2>

## 16-mask CMOS process

1. **Selecting a substrate**:

   Substrate is something on which you fabricate your complete design.

   There are various kind of substrate available but we will go for the most common one which we use for most of the mobile devices or any kind of device or chip you see in the real time --> **p-type**

   ![image](https://github.com/user-attachments/assets/0aa527d2-be4e-4c68-bd9b-67d6b690f93d)

2. **Creating active region for transistors**:

   1. Grow 40nm Silicon dioxide (SiO2) [act as an insulator] on the p-type substrate.

   2. Deposit a layer of 80nm Si3N4 over it.

   3. Deposit a layer of photoresist (1um) on top of it. Photoresist is a film, positive or negative film that see for old cameras. On this photoresist we are going to do some process.

   4. Mask1 --> When we talk about layouts those are nothing but mask in fabrication term. We basically protect some desired area through masking. In the below snippet that red color is masking. If there is UV light, then the area underneath those red masks are protected while the other resions are exposed to those UV light. So, we basically wash those resist area those are directly exposed to the UV light.

	![image](https://github.com/user-attachments/assets/3600eacd-2b5e-478d-b9ff-d02512ce520c)
  
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

3. **N-well and P-well formation**

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

4. **Formation of 'gate'**

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


5. **Lightly doped drain (LDD) formation**

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

6. **Source and Drain formation**

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


   




   


   

   




   



   





   



   





   

   



   











   

   






   



   

	


 

   


      


               


            


         


      
      


      





      





         

         


         


         



   

     


      

   




   












      







      

      

      


    


  

   





  
