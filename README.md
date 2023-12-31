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

 * The figure below represents the pictorial representation of how to access the excel sheet using the commands from he terminal.

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
  * **csv::read2matrix $f m, auto** ------ This command maps the opened csv file and the matrix that has been created. The comma is used as the channel separator and **auto** is to automatically identify the size of the matrix.
  * **close $f** ------ closes the opened csv file
  * **set columns [m columns]** ------ Returns the no. of columns for matrix m
  * **m link my_arr** -------- This command links the matrix 'm' to an array 'my_arr'.
  * **set no_of_rows [m rows]** ------ Returns the no. of rows for matrix m
  * **set i 0** ------ Provided for looping purpose.

### **TCL_D2_SK1 L4 - Auto creation of the first variable - DesignName**

  * The contents what we have till now is **$filename, $matrixName, $columns, $my_arr, $no_of_rows, $i**
  * **string map (_day _night) good_day** -------- Here the string map replaces **_day by _night**.

### **TCL_D2_SK1 L5 - Auto creation of variables complete**
  * **file normalize $my_arr(1, $i)** -------- Here this command will give the detailed path of the directory
    * **Before normalizaion** If the path would be **~/Desktop/vsdflow/vsdsynth**
    * **After normalization** the path would be **/home/shubha/Desktop/vsdflow/vsdsynth**

### **TCL_D2_SK1 L6 - Variable creation DEMO using TCL**

![variable_script](https://github.com/shubhagore/tclworkshop/assets/135098553/058428f2-d42a-4edf-bd0b-bc28bf1ed1da)

![variable_script1](https://github.com/shubhagore/tclworkshop/assets/135098553/d62456e9-158a-4cad-934b-7b506dbaf5b6)

![executing_vsdsynth_tcl](https://github.com/shubhagore/tclworkshop/assets/135098553/e324e82e-0987-46e7-b704-5f62f945ed6a)

![output_tcl1](https://github.com/shubhagore/tclworkshop/assets/135098553/ca104e0d-9760-4379-8b41-98f46507092f)

**Check if the **directories and paths** mentioned in the .csv file **exists or not****

  * We need to check if the mentioned files do exist or not, so here is the manual method of checking them.

![manual_check_of_files1](https://github.com/shubhagore/tclworkshop/assets/135098553/da76015e-6201-44c1-8394-84a2330dcf69)

![manual_check_of_files2](https://github.com/shubhagore/tclworkshop/assets/135098553/fc41197d-e5a3-4ffc-8a2f-3c832c0e569b)

![manual_check_of_files3](https://github.com/shubhagore/tclworkshop/assets/135098553/225cfbdd-bf50-4943-a325-5f014ca6838d)

## **TCL_D2_SK2 - Sub-Task Two-From CSV to format[1] and SDC-Processing constraints, CSV**
### **TCL_D2_SK2 L1 - Checking the existence of files and folders mentioned in design_details.csv**

  * The existence of file and directories should be done automatically using the script.

### **TCL_D2_SK2 L2 - Convert constraints.csv file to matrix object** 

  * The scripts for automation is as shown below

![file_check_script1](https://github.com/shubhagore/tclworkshop/assets/135098553/b7092d3a-6df1-4d43-9555-f7667b001d9b)

![file_check_script2](https://github.com/shubhagore/tclworkshop/assets/135098553/0123eeab-987f-4868-8532-b967e2f9725a)

  * Checking of existence of output directory is as below

![auto_check_of_files1](https://github.com/shubhagore/tclworkshop/assets/135098553/d243653f-5ec9-4731-87b7-e568a01e1dda)

![auto_check_of_files2](https://github.com/shubhagore/tclworkshop/assets/135098553/a68f31f9-76a8-41cd-a751-e89060a329b8)

![auto_check_of_files_output](https://github.com/shubhagore/tclworkshop/assets/135098553/3a9ddf95-08ec-419f-80fa-156b1d544305)

  * Some changes are been made in the excel sheet so that some files or directories with not found statements can be found

![opening_excel_file](https://github.com/shubhagore/tclworkshop/assets/135098553/19ca087b-18b1-451a-824c-53e80361dadf)

![excel_before_changing](https://github.com/shubhagore/tclworkshop/assets/135098553/d3bf46be-1b1c-46a9-ba93-48a43822967b)

![excel_after_changing](https://github.com/shubhagore/tclworkshop/assets/135098553/3b936ba4-baf4-46d3-8765-7d5e3fb11182)

  * The ouput after making changes in the excel sheet is as below

![output_tcl2](https://github.com/shubhagore/tclworkshop/assets/135098553/9e2fecaf-9e09-4298-ae27-5308c74be812)

**Read the "constraints file" for the above .csv and convert to SDC format.**

  * The constraints .csv file looks as below

![constraints_csv_file4](https://github.com/shubhagore/tclworkshop/assets/135098553/bb8b1e6e-1047-4132-ac85-6fad2520fdb3)

![constraints_csv_file2](https://github.com/shubhagore/tclworkshop/assets/135098553/a380ac19-1b12-48d4-a640-ba1eee9ceac2)

![constraints_csv_file3](https://github.com/shubhagore/tclworkshop/assets/135098553/5a828ae3-d411-44c2-a12b-e67ca724eb10)

  * In converting the .csv file to the SDC file the following steps need to be followed,
    * Convert the **csv to matrix**
    * Get the **count of rows and columns** of the matrix

### **TCL_D2_SK2 L3 - Compute row number using complex matrix processing**

  * The starting column number and row number of all the **clocks, input ports, output ports need to be calculated**.

### **TCL_D2_SK2 L4 - DEMO for computing row numbers**

  * The script to find the column number and row number of all the **clocks, input ports, output ports** is as shown below.

![row_column_no_csv_file_script](https://github.com/shubhagore/tclworkshop/assets/135098553/050a6081-ebcb-4eaa-b724-ce2746749f8e)

  * The output after calculating the row and column number is as shown below.

![row_column_no_csv_file_output1](https://github.com/shubhagore/tclworkshop/assets/135098553/e107c764-9015-4f03-8577-8b51012c3df2)

![row_column_no_csv_file_output2](https://github.com/shubhagore/tclworkshop/assets/135098553/9c73920b-fa75-456f-8a62-40a2cc6e0337)

  * In VLSI **delays are normally termed as LATENCY**

# **Day 3: Processing Clock and Input Constraints:**
## **TCL_D3_SK1 - Sub-Task Two-From CSV to format[1] and SDC- Processing clock constraints**
### **TCL_D3_SK1 L1 - Algorithm to identify the column number for clock latency constraints:**

### **TCL_D3_SK1 L2 - Start writing clock latency constraints in the SDC file:**

### **TCL_D3_SK1 L3 - Complete clock latency constraints and clockslew constraints in the SDC file:**

### **TCL_D3_SK1 L4 - Code to create clock constraints with clock period and duty cycle**

  * **Duty cycle = (frequency * duty cycle)/100**

### **TCL_D3_SK1 L5 - DEMO for creating complete clock constraints:**

  * The below figure shows the script for the clock constraints which is to be present in the SDC file

![clock_constraints_script1](https://github.com/shubhagore/tclworkshop/assets/135098553/40197b63-99d6-4249-ac4d-2698fc8a19cd)

![clock_constraints_script2](https://github.com/shubhagore/tclworkshop/assets/135098553/796dc077-d041-464c-90b9-9701e144c014)

  * If the above script is executed from the beginning then the output is as follows and a new SDC file will also be created in the path **/home/vsduser/vsdsynth/outdir_openMSP430**

![clock_constraints_output1](https://github.com/shubhagore/tclworkshop/assets/135098553/d43f3b33-9bf8-435d-82ec-f1eed35b4e79)

![clock_constraints_output2](https://github.com/shubhagore/tclworkshop/assets/135098553/c8771145-7262-4a09-a9a7-1ec6ad39431e)

  * The below figure is the SDC file that has been created after executing the the above mentioned script which is in the path **/home/vsduser/vsdsynth/outdir_openMSP430**.

![sdc_created](https://github.com/shubhagore/tclworkshop/assets/135098553/135a38a5-1c28-4eb8-a6d1-82f3a81a5f7a)

## **TCL_D3_SK2 - Sub-Task Two-From CSV to format[1] and SDC- Processing input constraints:**
### **TCL_D3_SK2 L1 - Introduction to the takof differentiating between bits and a bus:**

  * The multi-bit port is known as **bus**.
    * Example: **input [6:0] dbg_i2c_addr**
  
### **TCL_D3_SK2 L2 - Algorithm to categorize input ports as bits and bussed:**

  * The algorithm for differentiating the input ports as bits and bussed is as shown below,

![algorithm_input_ports](https://github.com/shubhagore/tclworkshop/assets/135098553/ab2a499a-5903-4a58-ae66-b2fb52ece7f0)

### **TCL_D3_SK2 L3 - File access and pattern creation steps**

  * **glob** means searching the wildcard in a particular direcory.

### **TCL_D3_SK2 L5 - Demo for grepping input ports from all verilogs and reformatting for fixed space**

![io_script1](https://github.com/shubhagore/tclworkshop/assets/135098553/b94cd9ff-7c1e-48be-92f3-a44546ddef0b)

![io_script2](https://github.com/shubhagore/tclworkshop/assets/135098553/04bf254c-5621-4fa1-85f7-d8614d8dcb22)

### **TCL_D3_SK2 L6 - Read, split, uniquify, sort, and join input ports to remove duplication:**

### **TCL_D3_SK2 L7 - Evaluate the length of the string and Demo of bits/bussed differentation script:**

### **TCL_D3_SK2 L8 - Demo for input constraints generation and bits/bussed differentiation:**

![io_script3](https://github.com/shubhagore/tclworkshop/assets/135098553/4fca3fc3-38e7-423f-a283-c444cf324930)

![io_script4](https://github.com/shubhagore/tclworkshop/assets/135098553/3091882a-af19-44e8-abb7-8d24f5205644)

![io_script5](https://github.com/shubhagore/tclworkshop/assets/135098553/5339cf1f-3d6c-4139-a10a-c44da4bce03e)

![io_script6](https://github.com/shubhagore/tclworkshop/assets/135098553/f0497760-09fc-4ef4-8c42-3ef861edcc69)

  * The SDC with input port is as below

![sdc_created_input_ports](https://github.com/shubhagore/tclworkshop/assets/135098553/7f8774e8-146e-4d5c-819b-ded0105ab95f)

# **Day 4: Complete Scriptingg and Yosys Synthesis Introduction:**
## **TCL_D4_SK1 - Full script for download and Conclusion:**
### **TCL_D4_SK1 L1 - Constraints generation logic for the output port and Conclusion!!:**

## **TCL_D4_SK2 - Introduction to Yosys synthesis tool and usage:**
### **TCL_D4_SK2 L1 - Example of a memory module RTL description:**

  * The yosys output is as below

![yosys_output](https://github.com/shubhagore/tclworkshop/assets/135098553/b1192c89-0297-47ba-8153-2aaa1b89b634)

### **TCL_D4_SK2 L2 - Memory functionality and Synthesis using Yosys:**

YOSYS is an open-source RTL synthesis and formal verification framework for digital circuits. It takes RTL descriptions (e.g., Verilog) as input and performs synthesis to generate a gate-level netlist. YOSYS supports technology mapping, optimization, and formal verification. It has a scripting interface, integrates with other EDA tools, and is widely used in academia and industry for digital design tasks.










