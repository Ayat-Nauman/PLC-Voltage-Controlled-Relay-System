**PLC Voltage-Controlled Relay System**  
A **Siemens LOGO! PLC**-based automation system that activates **24V relays** when analog voltage inputs (0-10V) exceed **2V threshold**, with 1:1 input-to-output mapping.

**Key Features**  
**3-Channel Voltage Monitoring** (0-10V range)  
**Threshold-Based Control** (2V activation point)  
**Direct I/O Mapping** (Input 1 → Relay 1, etc.)  
**Industrial-Grade Solution** using Siemens LOGO! PLC  

**Setup Instructions**  
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

**Technical Specifications**  
| Parameter        | Value              |
|------------------|--------------------|
| Input Voltage    | 0-10V DC           |
| Output Rating    | 24V DC, 10A relays |
| Control Logic    | Ladder Diagram     |
| PLC Model        | Siemens LOGO!      |

---

**Notes**:
1. The `/Software/` folder contains a text file with the official Siemens download link
2. The ladder logic file uses the `.lsc` extension standard for LOGO! Soft Comfort
3. No external dependencies required beyond the Siemens software
