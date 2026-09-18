# Telescopic Cascode Differential Amplifier Design

This project presents the design and simulation of a Telescopic Cascode Differential Amplifier using **TSMC 65-nm CMOS technology** with a 1.2V supply voltage. It was developed for the **Electronic Circuits 2 (ECE315)** course.

## Design Specifications (Required)
- **Minimum Voltage Gain**: > 500 (> 54 dB)
- **Maximum Power Consumption**: < 3 mW
- **Technology**: TSMC 65-nm CMOS
- **Methodology**: Simulation-driven $g_m/I_D$ methodology for accurate device sizing in deep-submicron technology.

## Achieved Results (Simulation)
- **Voltage Gain (Ao)**: 619.7 (55.84 dB)
- **Bandwidth (BW)**: 78.14 MHz
- **Gain-Bandwidth Product (GBW)**: 48.43 GHz
- **Power Consumption**: 91.11 µW
- **Phase Margin**: ~41°

## Key Features & Workflow
1. **LUT Generation**: DC sweeps to extract $g_m/I_D$, $g_m r_o$, and $I_D/W$ curves to relate biasing conditions to performance parameters.
2. **Sizing and Biasing**: Selected transistor dimensions and bias currents to ensure all transistors operate in saturation and achieve the desired transconductance efficiency.
3. **Simulation**: Extensive verification using Cadence Virtuoso:
   - **DC Analysis**: Verified operating points and output common-mode voltage setup.
   - **AC Analysis**: Verified differential small-signal gain (> 600) and frequency response.
   - **Phase Margin**: Evaluated stability, achieving ~41° phase margin.
4. **Robustness Testing**: 
   - **Corners Simulation**: Evaluated design over fast-slow, slow-fast, slow-slow, and fast-fast process corners.
   - **Monte Carlo Simulation**: Conducted 1000 statistical runs to analyze yield and variance in gain, bandwidth, and power consumption.

## Project Structure
- `Major_Task_Report.pdf`: Comprehensive report covering hand analysis, LUT charts, equations, and Cadence simulation results.
- `schematic.png`: Snapshot of the amplifier schematic.
- `schematic/`: Cadence Virtuoso schematic database files.

## Team Members
- Manar Saber Abdelrahim (22P0125)
- Mariam Islam Elsebaie (22P0177)
- Ahmed Sherif Mohamed (23P0414)

## Submitted To
- Prof. Sameh A. Ibrahim
