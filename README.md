# FPGA-BRAM-Voltage-Study

Characterization data collected on 4 FPGA platforms from Xilinx including a VC707, two identical samples of KC705, and a ZC702. You can find the background and analysis on the data in our MICRO'18 paper:

B. Salami, O. S. Unsal and A. Cristal Kestelman, "Comprehensive Evaluation of Supply Voltage Underscaling in FPGA on-Chip Memories," 2018 51st Annual IEEE/ACM International Symposium on Microarchitecture (MICRO), Fukuoka, Japan, 2019, pp. 724-736.
doi:10.1109/MICRO.2018.00064 


## Platform and Floorplan Information
This folder contains the default setting of each FPGA platform (default-setting.csv) as well as the floorplan of the BRAMs, i.e., physical location of BRAMs on the chip (floorplan.csv).

## Characterization Metholodolgy
Experiments are performed in normal ambient temperature from Vmin to Vcrash. Vmin is the supply voltage in which the first fault is observed. Vcrash is the supply voltage level beyond which the system crashes without any resonce. in the voltage guardband level (from the nominal to Vmin) there is no fault observed. 

## Fault Characterization Raw Data
This folder contains a sub-folder for each FPGA platform. Each sub-folder contains the raw content of BRAMs for each supply voltage level from Vmin to Vcrash with the steps of 0.01V. The file format is hex. The total number of faults is summarized in (platform-Fault.csv).  


