📘 12T SRAM Cell Design using Cadence Virtuoso
🔬 Overview

This repository contains the complete design, simulation, and analysis of a 12-Transistor (12T) Static Random Access Memory (SRAM) cell, implemented using Cadence Virtuoso.
The 12T architecture is an enhanced version of the classical 6T SRAM cell, offering improved stability, noise immunity, and robust operation in modern low-power and scaled CMOS technologies.

🎯 Project Objectives

Design a fully functional 12T SRAM cell

Implement separate read and write paths

Improve Static Noise Margin (SNM)

Achieve zero read disturbance

Evaluate performance at low supply voltages

Verify operation through DC, transient, and butterfly curve analysis

🧩 Why 12T SRAM?

Traditional 6T SRAM cells face challenges like read disturbance, poor SNM at low voltages, and higher sensitivity to process variations.
The 12T SRAM overcomes these limitations with:

✔ Dedicated Write Path

Prevents the read circuitry from interfering with write operations and improves write margin.

✔ Fully Isolated Read Path

The storage nodes remain untouched during read operations → zero read disturb.

✔ Higher SNM & Better Stability

Strong cross-coupled inverters and extra transistors create a more noise-resilient structure.

✔ Lower Leakage Power

Series stacking of transistors naturally reduces leakage currents.

🏗️ Design Flow
1. Schematic Design

Constructed cross-coupled inverters

Added write access transistors

Added dedicated read-buffer transistors

2. Transistor Sizing

Optimized PMOS/NMOS ratios

Balanced read/write margins

Maintained stable switching characteristics

3. Simulation

Performed using Virtuoso Analog Design Environment (ADE):

Transient analysis (write → hold → read)

DC operating point & VTC

Butterfly curve for SNM calculation

Parametric sweeps for voltage and sizing variations

4. Verification

Verified correct logic storage

Ensured no read disturb

Measured improved SNM over 6T cell

Checked leakage behavior at low VDD

📐 Results Included in This Repository

12T SRAM schematic

Simulation waveforms (read/write operations)

Noise margin analysis

Butterfly curve plots

Observations and performance comparisons

🚀 Applications

12T SRAM cells are used in systems demanding high reliability and stability, such as:

Low-power IoT devices

Near-threshold processors

AI accelerators

📌 Conclusion

This project demonstrates a complete custom 12T SRAM design cycle from schematic creation to performance validation.
The architecture provides superior stability, low-voltage reliability, and noise immunity, making it suitable for next-generation memory applications.

Aerospace & radiation-hardened designs

Ultra-scaled CMOS technologies
