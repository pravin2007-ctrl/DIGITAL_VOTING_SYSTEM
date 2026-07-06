# 🗳️ FPGA-Based Digital Voting System

A secure and efficient **Digital Voting System** implemented using **Verilog HDL** on an **FPGA** platform. The system enables authenticated voting, prevents duplicate votes, counts votes in real time, and displays election results through dedicated hardware logic.

---

## 📌 Overview

The FPGA-Based Digital Voting System is designed to provide a reliable and transparent electronic voting mechanism using digital hardware. Unlike software-based voting systems, the entire voting process is implemented in hardware, ensuring deterministic operation, low latency, and high reliability.

The system authenticates voters, records votes for multiple candidates, prevents multiple voting attempts, and displays the final vote count after the election.

---

## ✨ Features

- 🗳️ Electronic voting using FPGA
- ✅ One vote per voter
- 🔐 Duplicate vote prevention
- 📊 Real-time vote counting
- 👤 Multi-candidate support
- ⚡ Hardware-based implementation
- 🔄 Synchronous digital design
- 🧪 Testbench verification

---

## 🛠 Technologies Used

### Hardware

- FPGA Development Board
- Push Buttons / Switches
- LEDs
- Seven Segment Display

### Software

- Verilog HDL
- Xilinx Vivado Design Suite
- Vivado Simulator

---

## 🏗️ System Architecture

```
                 +------------------+
                 |   Voter Input    |
                 | Buttons/Switches |
                 +--------+---------+
                          |
                          ▼
               +----------------------+
               | Authentication Logic |
               +----------+-----------+
                          |
                          ▼
                +----------------------+
                | Duplicate Vote Check |
                +----------+-----------+
                          |
                          ▼
                +----------------------+
                | Vote Counter Module  |
                +----------+-----------+
                          |
          +---------------+---------------+
          |                               |
          ▼                               ▼
 +-------------------+          +--------------------+
 | Candidate Counters|          | Result Display     |
 +-------------------+          +--------------------+
```

---

## ⚙️ Working Principle

1. The system waits for a valid voter input.
2. The voter selects one of the available candidates.
3. Authentication logic verifies that the voter has not already voted.
4. If valid, the selected candidate's vote count is incremented.
5. Duplicate voting attempts are rejected.
6. Vote counts are updated in real time.
7. Final election results are displayed after voting ends.

---

## 📂 Project Structure

```
DIGITAL_VOTING_SYSTEM/
│
├── rtl/
│   ├── voting_controller.v
│   ├── vote_counter.v
│   ├── voter_auth.v
│   ├── display_controller.v
│   └── top_module.v
│
├── testbench/
│   └── tb_voting_system.v
│
├── constraints/
│   └── voting_system.xdc
│
├── simulation/
│
├── images/
│
└── README.md
```

---

## 🚀 Design Flow

```https://github.com/pravin2007-ctrl/DIGITAL_VOTING_SYSTEM
Voter Input
      │
      ▼
Authentication
      │
      ▼
Duplicate Vote Check
      │
      ▼
Vote Counter
      │
      ▼
Result Display
```

---

## 📊 System Features

| Feature | Description |
|----------|-------------|
| Authentication | Accepts only valid voting requests |
| Duplicate Prevention | Ensures one vote per voter |
| Vote Counting | Real-time hardware counting |
| Candidate Selection | Supports multiple candidates |
| Result Display | Displays live vote count |
| FPGA Implementation | Hardware-based execution |

---

## 💻 Getting Started

### Clone the Repository

```bash
git clone https://github.com/pravin2007-ctrl/DIGITAL_VOTING_SYSTEM.git
```

### Run the Project

1. Open Xilinx Vivado.
2. Create a new RTL project.
3. Add all Verilog source files.
4. Add the FPGA constraint (.xdc) file.
5. Run Simulation.
6. Run Synthesis.
7. Run Implementation.
8. Generate Bitstream.
9. Program the FPGA board.

---

## 📸 Results

The Digital Voting System was successfully simulated and implemented on FPGA hardware.

### Achievements

- ✔ Accurate vote counting
- ✔ Duplicate voting prevention
- ✔ Stable FPGA implementation
- ✔ Real-time result generation
- ✔ Reliable hardware operation

---

## 🎯 Applications

- College Elections
- Student Council Elections
- Organization Polling
- Small-Scale Elections
- Digital Survey Systems

---

## 🔮 Future Enhancements

- Fingerprint authentication
- RFID-based voter identification
- Biometric verification
- Secure result storage
- Wireless result transmission
- IoT-based election monitoring
- Blockchain integration for audit trails
- Touchscreen interface

---

## 👨‍💻 Author

**Pravin A**  
B.E. Electronics and Communication Engineering

GitHub: https://github.com/pravin2007-ctrl


---

## ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub to support future development.
