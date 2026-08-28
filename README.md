# Automated Manufacturing Line – Siemens TIA Portal & Factory I/O

This project is a simulated automated manufacturing line using Siemens TIA Portal, S7-PLCSIM, and Factory I/O.

The line handles parts through different stages including feeding, machining, material transfer, sorting, and assembly. The PLC controls the sequence based on sensor feedback and sends commands to conveyors, actuators, and pick-and-place mechanisms.

I used Factory I/O to simulate the physical production line and S7-PLCSIM to run and test the PLC program without a physical PLC.

## Software

- Siemens TIA Portal V16
- S7-PLCSIM V16
- Factory I/O
- Ladder Logic
- Siemens HMI

## What the System Does

The PLC controls the production line step by step.

Sensors are used to detect when parts reach different positions in the line. Based on those signals, the PLC starts or stops conveyors, runs machining operations, and controls the pick-and-place sequence.

The program also uses interlocks so that two conflicting operations cannot run at the same time and each step has to finish before the next step starts.

The system includes:

- Part feeding
- Conveyor control
- Pick-and-place operations
- Machining stations
- Product transfer
- Sorting
- Assembly
- HMI control and monitoring
- Start/Stop control
- Emergency stop logic
- Sequence interlocks
- Fault handling

## PLC Program

I separated the control logic into different function blocks based on the operation being controlled.

This makes the program easier to follow, test, and troubleshoot instead of putting the whole production sequence into one block.

The PLC logic handles:

- Sensor conditions
- Motor and conveyor commands
- Robot movement sequences
- Machining operations
- Part tracking
- Interlocks
- Operating conditions
- Fault conditions

<img width="1910" height="1004" alt="Screenshot 2026-08-27 194249" src="https://github.com/user-attachments/assets/f2174e6b-98ea-4f65-89f9-58a8cd86029a" />
<img width="1910" height="1028" alt="Screenshot 2026-08-27 195227" src="https://github.com/user-attachments/assets/f68f5ddc-f268-4fc3-92e6-e6f768e3f041" />

## Factory I/O Integration

Factory I/O is connected to the simulated PLC through S7-PLCSIM.

The inputs from Factory I/O, such as sensors and push buttons, are mapped to PLC input addresses.

PLC outputs are mapped back to Factory I/O to control things such as:

- Conveyors
- Actuators
- Pick-and-place mechanisms
- Machining stations
- Indicators

This allowed me to test the full PLC sequence in a 3D environment before using any physical hardware.

<img width="1898" height="1019" alt="Screenshot 2026-08-27 193601" src="https://github.com/user-attachments/assets/b781e35b-935d-43ba-b945-17ea2dc93fef" />


## HMI

The HMI is used to monitor and control the production line.

It provides access to the main operating controls and gives the operator information about the current state of the system.

Depending on the operating condition, the HMI can be used to:

- Start and stop the line
- Monitor equipment status
- View system conditions
- Identify faults

<img width="1910" height="1029" alt="Screenshot 2026-08-27 193949" src="https://github.com/user-attachments/assets/ac69f2c8-19fc-4236-b5b1-33bf2e65506b" />
<img width="1910" height="1025" alt="Screenshot 2026-08-27 195429" src="https://github.com/user-attachments/assets/29d5450c-aafb-4358-9570-71a43bf3d453" />


## project video link

[https://drive.google.com/drive/folders/1QvybJ1SnndVTOGTmAKarzBqqVmDQEwEX](https://drive.google.com/drive/folders/1QvybJ1SnndVTOGTmAKarzBqqVmDQEwEX)
