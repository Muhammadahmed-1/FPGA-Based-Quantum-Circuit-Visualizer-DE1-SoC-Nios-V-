# Quantum Circuit Simulator / Visualizer (DE1-SoC)

Design, simulate, and **visualize quantum circuits** on an FPGA. Place gates on qubit lines via PS/2 keyboard, see the layout on VGA, then run the simulation to view **measurement results** and **Bloch sphere** states. Includes audio feedback and hardware button controls.

##  System Overview
https://cpulator.01xz.net/?sys=rv32-de1soc 

### Block Diagram
<img width="1040" height="550" alt="image" src="https://github.com/user-attachments/assets/059e3a7d-eb20-4a2a-908f-069020a2dd56" />

[🎥 Intro Video](https://drive.google.com/file/d/1zs84S7syiwwLpPiYiG_ydYeDh8zNORlE/view?usp=sharing)  
[🎥 Demo Video](https://drive.google.com/file/d/1X59DS0ua7ZcYQfr9I3pKQoOaoxn_Hf03/view?usp=sharing)

---
<img width="883" height="568" alt="image" src="https://github.com/user-attachments/assets/dda16662-76c2-4d4c-9580-08441a5d6499" />

##  Features

- **Interactive Circuit Design**
  - Place gates (H, X, Z, CNOT, …) using the **PS/2 keyboard**
  - Toggle qubit initial states with **push buttons**
  - Live **VGA** circuit rendering (start screen → circuit editor → output pages)

- **Simulation & Visualization**
  - **R** to run the circuit and show final measurement results
  - **B** to render **Bloch sphere** visualization
  - Prints measured probabilities to the **terminal (UART/JTAG)**

- **UX / Feedback**
  - **Audio** cue on interactions (gate placement, transitions)
  - **ESC / Backspace** to reset and return to the circuit page

---

##  Quick Navigation (Controls)

| Action                               | Input                          |
|--------------------------------------|--------------------------------|
| Start (go to Circuit page)           | `KEY0` (push button)          |
| Toggle initial state of a qubit line | On-board **push buttons**      |
| Place gate on a qubit                | `qubit_index` → `GateKey` → `Enter`  |
| Example (H on qubit 0)               | `0` → `H` → `Enter`            |
| Run simulation                       | `R`                            |
| Show Bloch sphere                    | `B`                            |
| Reset / Back                         | `ESC` or `Backspace`           |

> Gate keys (example): `H`, `X`, `Z`, `C` (CNOT), …  
---

