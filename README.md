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


# **Day 1: Introduction to TCL and VSDSYNTH Toolbox Usage:**
## **TCL_D1_SK1 - Introduction**
### **TCL_D1_SK1 L0 - Introduction to TCL task:**
 * The task is **to build a user-interface that will take Excel sheet as the input and will provide the output as the datasheet**.
 * The excel sheet consists of some important characteristics of our design such as **design name, output directory, netlist directory, Early library path, late library path, constraints file**, etc.

![ex_sheet_content](https://github.com/shubhagore/tclworkshop/assets/135098553/0111c9e6-90e8-4c87-ba1f-94b6c505243c)

 * The figure below represents the pictorial representation of hoe to access the excel sheet using the commands from he terminal.

![excel_opening_command](https://github.com/shubhagore/tclworkshop/assets/135098553/bc635822-9f35-4ed2-896f-969f304b5870)

 * The below figure shows the pictorial representation of the task in the workshop. The **TCL box** in the figure below is the **User interface** that we need to design.
 
![workshop_task](https://github.com/shubhagore/tclworkshop/assets/135098553/231b457f-4ab0-436c-8a89-e3805388cf93)

![workshop_task1](https://github.com/shubhagore/tclworkshop/assets/135098553/924d9991-2ee7-4088-95ef-403b91a9a238)

### **TCL_D1_SK1 L1 - Introduction to sub-task:** 
 * We are aware of the main task. We need to divide the main task into sub-task. This process of dividing the task from the main task is known as **top down approach**.
 * The list of sub-tasks is as follows,
   * Create the command (eg: vsdsynth) and pass .csv from UNIX to TCL script.(We need to create a command to which .csv file is given as the input).

![subtask1](https://github.com/shubhagore/tclworkshop/assets/135098553/e396041e-e769-4444-ae1e-f49572f2dc75)

   * Convert all the inputs to format[1] and SDC format and pass to synthesis tool "**yosys**".
   * Convert all the inputs to format[1] and SDC to format[2] and pass to the timing tool **"opentimer"**.
   * Generate the output report.

## **TCL_D1_SK2 - Sub-Task One: VSDSYNTH Toolbox usage scenarios**
### **TCL_D1_SK2 L1 - Scenario 1 - User doesn't provide an input CSV file:** 
 
 * The first tasknow is to **Create the command (eg: vsdsynth) and pass .csv from UNIX to TCL script.**
 * We will note some of the scenarios from the user point of view
   * User might not be provided by the .csv file as the input by mistake. At that time we have to go back to the user requesting to provide them the .csv file.
   * The user might have provided the .csv file, but the .csv file doesn't exists in the current working directory. But the vsdsynth block shouldn't stop and keep notifying or popping the error as .csv file doesn't exits.
   * User just wants to know how to run this UI, thus user may type **"-help"**

![user_scenarios](https://github.com/shubhagore/tclworkshop/assets/135098553/692a6892-7b61-430a-81ca-a88f2a46ed07)

#### **User might not be provided by the .csv file as the input:**

  * Check for the arguments provided along with **./vsdsynth {arg1}  {arg2} {arg3}...**. The argument count should always be atleast **1**. If the **arg != 1** then an echo statement will be printed saying **Please provide the .csv file**.

![arguments](https://github.com/shubhagore/tclworkshop/assets/135098553/57958960-4856-4799-996c-cf3f42eaf4ab)

##### **Create Command (TCL) and pass csv file from UNIX shell to Tcl script**
  * Open a script file here **eg vsdsynth**.

![opening_vsdsynth_file](https://github.com/shubhagore/tclworkshop/assets/135098553/a8973983-b8bb-4e02-9db1-7f5e15bfb941)
   
  * The picture below represent the script informing to provide the .csv file.

![provide_csv](https://github.com/shubhagore/tclworkshop/assets/135098553/554f3b68-8736-48e8-9faf-4e1beb9facd0)

![vsdsynth_file](https://github.com/shubhagore/tclworkshop/assets/135098553/fee11f9e-b4de-4ea5-9410-e34edfcc696f)

  * The vsdsynth file doesn't have executable permission so need to change to executable file.

 ![change_of_permission](https://github.com/shubhagore/tclworkshop/assets/135098553/9504b735-8e54-47d8-806a-be78e93928af)

  * Executing the vsdsyth using the command **./vsdsynth**.

![executing_vsdsynth](https://github.com/shubhagore/tclworkshop/assets/135098553/55a2eca2-24c1-492b-bccc-717566120d6b)

### **TCL_D1_SK2 L2 - Scenarios 2 & 3 - User providing incorrect CSV or typing "-help":**

#### **The user might have provided the .csv file, but the .csv file doesn't exists in the current working directory:**

  * The script for finding if the provided input file doesn't exists is as below

![script_for_csv_dont_exist](https://github.com/shubhagore/tclworkshop/assets/135098553/6c5f2175-3111-4f16-b17e-1a6fdf866481)

  * Executing the vsdsynth file by passing the incorect .csv file.

![csv_dont_exist](https://github.com/shubhagore/tclworkshop/assets/135098553/303f1e9c-c175-4321-bbab-afd61f574c0c)

#### **User just wants to know how to run this UI, thus user may type **"-help"**:**
  * The script for the execution if the user has typed **-help** is as shown below.

![script_for_wrong_csv_and_help](https://github.com/shubhagore/tclworkshop/assets/135098553/0334f094-15a4-4df9-899e-cac5c2fd2d90)

  * Executing vsdsynth with **-help** as the argument.

![output_help1](https://github.com/shubhagore/tclworkshop/assets/135098553/605d6619-c226-48fa-8bba-8e7202c3c433)

![output_help2](https://github.com/shubhagore/tclworkshop/assets/135098553/405b498c-384a-4f2f-afcb-0506f92bbbf7)


# **Day 2: Variable creation and Processing Constraints from CSV:**
## **TCL_D2_SK1 - Sub-Task Two-From CSV to format[1] and SDC-Variable Creation**
### **TCL_D2_SK1 L1 - Various tasks involved in format conversion:**
 
 **Convert all the inputs to format[1] and SDC format and pass to synthesis tool "**yosys**"**  
 
 * There are further sub-tasks for easy understanding
    * **Creating the variables**, so that the paths present in the excel can be accessed using these variables.
    * Check if the **directories and paths** mentioned in the .csv file **exists or not**
    * Read the **"constraints file"** for the above .csv and **convert to SDC** (Standard synopsys design constraints) format.
    * Read all the files in the **"Netlist directory"**.
    * Create the main **synthesis script in format[2]**
    * Pass this script to **"Yosys"**.

### **TCL_D2_SK1 L2 - Auto-Create variables using matrix and arrays:**

**Convert all the inputs to format[1] and SDC format and pass to synthesis tool "**yosys**"**  
**Creating the variables**

  * Now we are aware of how to pass the .csv file into vsdsynth file (shell script file) and way to access the .csv is using **tclsh ./vsdsynth.tcl $argv[1]**.
  * Next step is to access the elements of .csv file what we have
  * The below figure gives the pictorial represenatation of accessing the .csv file in the form of arguments

![acess_argv](https://github.com/shubhagore/tclworkshop/assets/135098553/3ec20001-a897-403d-8e1d-7f2a8ebbf0ae)

  * In the above figure the **lindex** is a TCL command which will help in listing the index when there are lists of arguments.
  * Steps involved in creating the variables out of the csv file is
    * Convert the contents of **.csv file into a matrix**. To access the matrix we need to know the number of rows and columns of a matrix. **matrix(column,row)** is the format.
    * Convert the **matrix into an array**.  

![processing](https://github.com/shubhagore/tclworkshop/assets/135098553/0f989187-fcb4-4250-b59e-983d707c058f)

### **TCL_D2_SK1 L3 - Initialize variables for auto-creation variables task:**
  * Initially we will have to **set the filname**.
  * Create the matrix object and the command used is **struct::matrix m**. The **two packages** are required to **process a csv and a matrix**. Hence they should be mentioned.
  * **set f [open $filename]** ----- This indicates that the variable 'f' is assigned to the opened file in read mode. This command is equivalent to vim in linux
  * **csv::read2matrix $f m, auto** ------ This command maps the opened csv file and the matrix that has been created. 










