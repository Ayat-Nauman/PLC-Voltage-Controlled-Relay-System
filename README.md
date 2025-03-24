Here's the refined **GitHub README** with your requested repository structure changes:

# **GitHub README for PLC Voltage-Controlled Relay System**  

## **Project Overview**  
A **Siemens LOGO! PLC**-based automation system that activates **24V relays** when analog voltage inputs (0-10V) exceed **2V threshold**, with 1:1 input-to-output mapping.

### **Repository Structure**  
```
/plc-voltage-relay-control/
│── /Software/
│   └── Siemens_LOGO_Software_Download.txt  # Contains download link for LOGO! Soft Comfort
│── /Schematic/
│   └── Wiring_diagram.jpg  # Contains wiring diagram of the ladder logic
│── /Program/
│   └── Voltage_Relay_Logic.lsc            # Complete ladder logic program
│── README.md                              # This documentation file
```

## **Key Features**  
✔ **3-Channel Voltage Monitoring** (0-10V range)  
✔ **Threshold-Based Control** (2V activation point)  
✔ **Direct I/O Mapping** (Input 1 → Relay 1, etc.)  
✔ **Industrial-Grade Solution** using Siemens LOGO! PLC  

## **Setup Instructions**  
1. **Software Installation**  
   - Download LOGO! Soft Comfort from link in `/Software/` folder  
   - Install on Windows PC  

2. **Program Deployment**  
   - Open `Voltage_Relay_Logic.lsc` in LOGO! Soft Comfort  
   - Connect to LOGO! PLC via USB/PROFIBUS  
   - Transfer program to PLC  

3. **Hardware Connections**  
   ```
   Analog Inputs (0-10V):
   - AI1 → Voltage Source 1
   - AI2 → Voltage Source 2  
   - AI3 → Voltage Source 3
   
   Relay Outputs (24V):
   - Q1 → Relay 1 Load
   - Q2 → Relay 2 Load
   - Q3 → Relay 3 Load
   ```

## **Technical Specifications**  
| Parameter        | Value              |
|------------------|--------------------|
| Input Voltage    | 0-10V DC           |
| Output Rating    | 24V DC, 10A relays |
| Control Logic    | Ladder Diagram     |
| PLC Model        | Siemens LOGO!      |

## **Resume One-Liner**  
**Industrial Relay Control System (Siemens LOGO! PLC)** - Developed ladder logic program for voltage-controlled relay activation with 2V threshold detection and 3-channel independent control.

---

### **Notes**:
1. The `/Software/` folder contains a text file with the official Siemens download link
2. The ladder logic file uses the `.lsc` extension standard for LOGO! Soft Comfort
3. No external dependencies required beyond the Siemens software

This structure keeps your repository minimal yet complete, focusing on the two key components you specified (software link and program file) while maintaining professional documentation.
