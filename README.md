# Synopsys VLSI Flow — RTL to GDSII (Hands-on Learning)

Overview

This repository documents a hands-on learning journey through the Synopsys digital design flow, covering the full RTL-to-GDSII process: RTL synthesis, static timing analysis (STA), place-and-route (PnR), and GDSII generation. The goal is to provide reproducible examples, scripts, notes, and reports to help learners and engineers practice and understand the flow.

Repository structure

- rtl/        — example RTL (Verilog/VHDL) sources
- synth/      — synthesis scripts, Synopsys Design Compiler configs, synthesis reports
- pnr/        — place-and-route scripts, floorplans, PnR reports (IC Compiler / Fusion Compiler)
- sta/        — static timing scripts and PrimeTime reports
- gds/        — layout exports and GDSII files
- docs/       — step-by-step guides, tips, and notes
- scripts/    — helper scripts (automation, parsing, environment setup)
- tests/      — example testbenches or smoke tests

Quick start

1. Prerequisites
   - Synopsys tools (Design Compiler, IC Compiler/Fusion Compiler, PrimeTime)
   - Linux environment (bash)
   - Adequate licenses and access to foundry PDKs if running full PnR/GDS flows

2. Prepare environment
   - export SYNOPSYS_HOME=/path/to/synopsys
   - source $SYNOPSYS_HOME/setup.sh
   - Ensure PATH and LM_LICENSE_FILE (or other license variables) are set correctly

3. Example run
   - Synthesis:
     cd synth
     ./run_synth.sh <design>
   - Place & Route:
     cd pnr
     ./run_pnr.sh <design>
   - Static Timing Analysis:
     cd sta
     ./run_sta.sh <design>

Notes

- Many scripts are intended as examples and may need adjustments for your tool versions, PDK, or compute environment.
- For any step that accesses licensed tools or PDKs, make sure you have the appropriate permissions and environment variables configured.

Contributing

Contributions are welcome. Please open issues for problems or suggestions and submit pull requests for improvements. When contributing, include:

- The tool versions you used
- The platform/OS
- A brief description of the change and why it helps reproducibility

Maintainer: SandeepSingh8769
