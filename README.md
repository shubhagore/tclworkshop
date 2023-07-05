# **TCL WORKSHOP**

# **Table of content**

# **Day 1: Introduction to TCL and VSDSYNTH Toolbox Usage:**
## * TCL_D1_SK1 - Introduction
  * TCL_D1_SK1 L0 - Introduction to TCL task
  * TCL_D1_SK1 L1 - Introduction to sub-task
## * TCL_D1_SK2 - Sub-Task One: VSDSYNTH Toolbox usage scenarios
  * TCL_D1_SK2 L1 - Scenario 1 - User doesn't provide an input CSV file
  * TCL_D1_SK2 L2 - Scenarios 2 & 3 - User providing incorrect CSV or typing "-help"

# **Day 2: Variable creation and Processing Constraints from CSV:**
## * TCL_D2_SK1 - Sub-Task Two-From CSV to format[1] and SDC-Variable Creation
  * TCL_D2_SK1 L1 - Various tasks involved in format conversion
  * TCL_D2_SK1 L2 - Auto-Create variables using matrix and arrays
  * TCL_D2_SK1 L3 - Initialize variables for auto-creation variables task
  * TCL_D2_SK1 L4 - Auto creation of the first variable - DesignName
  * TCL_D2_SK1 L5 - Auto creation of variables complete
  * TCL_D2_SK1 L6 - Variable creation DEMO using TCL
## * TCL_D2_SK2 - Sub-Task Two-From CSV to format[1] and SDC-Processing constraints, CSV
  * TCL_D2_SK2 L1 - Checking the existence of files and folders mentioned in design_details.csv
  * TCL_D2_SK2 L2 - Convert constraints.csv file to matrix object
  * TCL_D2_SK2 L3 - Compute row number using complex matrix processing
  * TCL_D2_SK2 L4 - DEMO for computing row numbers
# **Day 3: Processing Clock and Input Constraints:**
## * TCL_D3_SK1 - Sub-Task Two-From CSV to format[1] and SDC- Processing clock constraints
  * TCL_D3_SK1 L1 - Algorithm to identify the column number for clock latency constraints
  * TCL_D3_SK1 L2 - Start writing clock latency constraints in the SDC file
  * TCL_D3_SK1 L3 - Complete clock latency constraints and clockslew constraints in the SDC file
  * TCL_D3_SK1 L4 - Code to create clock constraints with clock period and duty cycle
  * TCL_D3_SK1 L5 - DEMO for creating complete clock constraints
## * TCL_D3_SK2 - Sub-Task Two-From CSV to format[1] and SDC- Processing input constraints
  * TCL_D3_SK2 L1 - Introduction to the takof differentiating between bits and a bus
  * TCL_D3_SK2 L2 - Algorithm to categorize input ports as bits and bussed
  * TCL_D3_SK2 L3 - File access and pattern creation steps
  * TCL_D3_SK2 L4 - Regular expression and regular substitute to get fixed space strings
  * TCL_D3_SK2 L5 - Demo for grepping input ports from all verilogs and reformatting for fixed space
  * TCL_D3_SK2 L6 - Read, split, uniquify, sort, and join input ports to remove duplication
  * TCL_D3_SK2 L7 - Evaluate the length of the string and Demo of bits/bussed differentation script
  * TCL_D3_SK2 L8 - Demo for input constraints generation and bits/bussed differentiation
# **Day 4: Complete Scriptingg and Yosys Synthesis Introduction:**
## * TCL_D4_SK1 - Full script for download and Conclusion
  * TCL_D4_SK1 L1 - Constraints generation logic for the output port and Conclusion!!
## * TCL_D4_SK2 - Introduction to Yosys synthesis tool and usage
  * TCL_D4_SK2 L1 - Example of a memory module RTL description
  * TCL_D4_SK2 L2 - Memory functionality and Synthesis using Yosys
  * TCL_D4_SK2 L3 - Components and Gate level netlist description of Synthesized memory
  * TCL_D4_SK2 L4 - Memory write operation discussed in detail
  * TCL_D4_SK2 L5 - Memory read operation and TCL scripting agenda
## * TCL_D4_SK3 - Hierarchy check and error handling script creation for Yosys
  * TCL_D4_SK3 L1 - Script to do hierarchy check 
  * TCL_D4_SK3 L2 - Demo for hierarchy check script generation
  * TCL_D4_SK3 L3 - Demo for error handling concpt in hierarchy check
  * TCL_D4_SK3 L4 - Error handling script forhierarchy check
  * TCL_D4_SK3 L5 - Demo for error handling script
# **Day 5: Advanced Scripting Techniques and Quality of Results generation:**
## * TCL_D5_SK1 - Synthesis main file scripting and output file editing
  * TCL_D5_SK1 L1 - Synthesis script creation and demo
  * TCL_D5_SK1 L2 - Need and script to edit Yosys output netlist
  * TCL_D5_SK1 L3 - Demo to edit output netlist and Introduction to 'procs'
## * TCL_D5_SK2 - World of 'Procs'
  * TCL_D5_SK2 L1 - Redirect stdout proc and demo of TCL array command
  * TCL_D5_SK2 L2 - 'set_multi_cpu_usage' proc
  * TCL_D5_SK2 L3 - Demo for 'set_multi_cpu_usage' proc
  * TCL_D5_SK2 L4 - read_lib and read_verilog proc demo
## * TCL_D5_SK3 - read_sdc proc interpret clock generation constraints
  * TCL_D5_SK3 L1 - Read SDC file and replace square brackets by 'null'
  * TCL_D5_SK3 L2 - Evaluate clock period and clodk port name from processed SDC
  * TCL_D5_SK3 L3 - Evaluate duty cycle and create clock in opentimer format
  * TCL_D5_SK3 L4 - Demo to convert constraints from SDC format to opentimer format
## * TCL_D5_SK4 - read_sdc proc interpret IO Delays and transition constraints
  * TCL_D5_SK4 L1 - Grep clock latency and port name from SDC file
  * TCL_D5_SK4 L2 - Convert set_clock_latency SDC to opentimer format
  * TCL_D5_SK4 L3 - Demo to convert set_clock_latency in SDC to arrival_time in opentimer
  * TCL_D5_SK4 L4 - Script and demo to convert transition and input delay to opentimer format
  * TCL_D5_SK4 L5 - Script and demo to convert output SDC constraints to opentimer format
## * TCL_D5_SK5 - Process bussed ports and configuration file creation
  * TCL_D5_SK5 L1 - Script to expand bussed input ports for arrival time constraints
  * TCL_D5_SK5 L2 - Script and demo to convert all bussed constraints to bit-blasted
  * TCL_D5_SK5 L3 - Opentimer configuration file creation  
## * TCL_D5_SK6 - Quality of results (QOR) generation algorithm
  * TCL_D5_SK6 L1 - Script to obtain STA runtime
  * TCL_D5_SK6 L2 - Script to obtain WNS and FEP for reg2out violations
  * TCL_D5_SK6 L3 - Script and demo for instance count, WNS and FEP fo setup and hold
  * TCL_D5_SK6 L4 - Script and demo for reportt formatting
## * TCL_D5_SK7 - Conclusion
  * TCL_D5_SK7 L1 - Conclusion and acknowledgments











