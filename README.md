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


    


  

   





  
