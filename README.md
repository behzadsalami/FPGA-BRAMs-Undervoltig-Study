# FPGA BRAMs-Voltage-Study

Characterization data collected on 4 FPGA platforms from Xilinx including a VC707, two identical samples of KC705, and a ZC702. You can find the background and analysis on the data in our MICRO'18 paper:

B. Salami, O. S. Unsal and A. Cristal Kestelman, "Comprehensive Evaluation of Supply Voltage Underscaling in FPGA on-Chip Memories," 2018 51st Annual IEEE/ACM International Symposium on Microarchitecture (MICRO), Fukuoka, Japan, 2019, pp. 724-736.
doi:10.1109/MICRO.2018.00064 

## Metholodolgy
Experiments are performed in normal ambient temperature from Vmin to Vcrash. Vmin is the supply voltage in which the first fault is observed. Vcrash is the supply voltage level beyond which the system crashes without any resonce. Vmin and Vcrash are slightly different for different platforms. In the voltage guardband level (from the nominal= 1V to Vmin) no fault is observed. 

## Fault Characterization
This folder contains a sub-folder for each FPGA platform. Each sub-folder contains two types of files. 

First, "information.csv" contains information for each platform including the floorplan of the BRAMs, i.e., physical location of BRAMs on the chip, default setting, and the total number of faults in different voltage levels. 

Second, there is a folder (RawData) that contains the raw content of BRAMs for each supply voltage level from Vmin to Vcrash with the steps of 0.01V. The file format is hex and any '0' represents a 1-to-0 bit-flip in the corresponding location of the given BRAMs. 

