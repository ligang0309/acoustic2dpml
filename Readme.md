# ACOUSTIC2DPML

ACOUSTIC2DPML is a MATLAB package designed for 2D frequency-domain acoustic wavefield simulations. It implements both the conventional 9-point finite-difference scheme (Jo et al., 1996) and the recently developed 17-point scheme (Cao and Chen, 2012), utilizing optimized Convolutional Perfectly Matched Layer (CFS-PML) boundary conditions.

> **Note:** The original paper presenting the 17-point scheme by Cao and Chen (2012) was published in Chinese. This package provides a MATLAB implementation of the 17-point scheme integrated with our optimized CFS-PML boundary. Readers are referred to our publication in *GEOPHYSICS* for detailed methodology.

## References

For details regarding the finite-difference schemes employed, please consult the following literature:

*   Jo, C.-H., Shin, J.-H., and Suh, J.-H., 1996, An optimal 9-point finite-difference frequency-space 2-D scalar wave extrapolator: *Geophysics*, 61(2), 529–537.
*   Cao, S.-H., and Chen, J.-B., 2012, A 17-point scheme and its numerical implementation for high-accuracy modeling of frequency-domain acoustic equation: *Chinese Journal of Geophysics* (in Chinese), 55(10), 3440–3449.

---

## 1. Code Overview

The main executable script is located in the `/SourceCode` subdirectory:

*   **`acoustic2dpml.m`**: Primary script to run the simulation.

### Input Files and Output Results
Refer to the `Readme.txt` file within the `/Examples` subdirectory for specifications regarding input formats and output data.

---

## 2. Directory Structure

### 2.1 `/SourceCode`
Contains all MATLAB source codes for the package.

### 2.2 `/Examples`
Contains test cases for homogeneous, Overthrust, and Marmousi2 models, along with corresponding figures generated during this study.

---

## 3. Usage Declaration

ACOUSTIC2DPML is distributed exclusively for **academic use only**. THE SOFTWARE IS PROVIDED "AS IS", **WITHOUT WARRANTY OF ANY KIND**, express or implied, including but not limited to the warranties of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. Users should retain a copy of the GNU License or the SEG `disclaimer.txt` file included in this package. For more details, see the [GNU License](https://www.gnu.org/licenses/) and the [SEG Disclaimer](https://software.seg.org/disclaimer.txt).

### External Packages Used
*   **`wigb.m`**: A plotting utility distributed freely for academic use.
    *   Source: [https://github.com/nicklinyi/seismic_utils/blob/master/wigb.m](https://github.com/nicklinyi/seismic_utils/blob/master/wigb.m)
*   **`balance_trace.m`**: Utility for trace balancing located in `/Examples/Marmousi2/Seismograms/`.
    *   Author: Yutao Liu
    *   Affiliation: Science & Technology on Integrated Information System Laboratory, Institute of Software, Chinese Academy of Sciences, Beijing, China
    *   E-mail: yutao_liu2022@163.com

### Citation Requirement
If you present results derived from ACOUSTIC2DPML in a publication or presentation, please cite the following paper:

> Lei, W., Liu, Y., Li, G.*, Zhu, S., Chen, G., & Li, C.-F., 2023, 2D frequency-domain finite-difference acoustic wave modeling using optimized perfectly matched layers: *Geophysics*, 88(2), F1–F13. DOI: [10.1190/geo2022-0145.1](https://doi.org/10.1190/geo2022-0145.1)

---

## Contact

For questions or support, please contact the developers:

**Wen Lei** / **Dr. Gang Li***
Department of Marine Sciences, Zhejiang University
*Email:* [gangli@zju.edu.cn](mailto:gangli@zju.edu.cn) / [ligang0309@gmail.com](mailto:ligang0309@gmail.com)