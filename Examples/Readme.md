# Examples Documentation

This directory contains test cases for the **Homogeneous**, **Overthrust**, and **Marmousi2** models, along with their associated figures.

---

## 1. Running the Simulations

### 1.1 Parameter Settings
To run a test (e.g., the Homogeneous model), modify the configuration file located in the specific `Inputs` subfolder. For example:
`/acoustic2dpml/Examples/Homogeneous/Inputs/para9_optimizedCFSPML.txt`

This specific file configures the simulation to use the **9-point scheme** combined with our **optimized CFS-PML** boundary conditions.

The parameters are defined line-by-line in the text file as follows:

1.  **Number of grid nodes in the X-direction**
2.  **Number of grid nodes in the Z-direction**
3.  **Number of absorption layers in the X-direction**
4.  **Number of absorption layers in the Z-direction**
5.  **Grid spacing** (spatial sampling interval)
6.  **Finite-Difference Scheme Type**:
    *   `0`: 9-point scheme
    *   `1`: 17-point scheme
7.  **Absorbing Boundary Type**:
    *   `0`: Conventional PML
    *   `1`: CFS-PML
    *   `2`: Optimized CFS-PML
8.  **Frequency slice interval**

#### Available Configuration Files
Use the following files to switch between different schemes and boundary conditions:

*   `para9_PML.txt`: 9-point scheme, Conventional PML
*   `para9_CFSPML.txt`: 9-point scheme, CFS-PML
*   `para9_optimizedCFSPML.txt`: 9-point scheme, Optimized CFS-PML
*   `para17_PML.txt`: 17-point scheme, Conventional PML
*   `para17_CFSPML.txt`: 17-point scheme, CFS-PML
*   `para17_optimizedCFSPML.txt`: 17-point scheme, Optimized CFS-PML

### 1.2 Velocity Model Files
The velocity model file for the homogeneous test is named `Homo.mesh`.

---

## 2. Results and Plotting

Simulation outputs and plotting scripts are organized into subdirectories based on the model type:

*   **Seismograms**: Located in `/Examples/[ModelName]/Seismograms/`
*   **Snapshots**: Located in `/Examples/[ModelName]/Snapshots/`

Please refer to the `Readme.md` file within these specific subfolders for detailed instructions regarding output formats and visualization procedures.