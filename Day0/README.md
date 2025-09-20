# Day 0 — Tools Installation

Today, I set up my entire environment for the **RISC-V SoC Tapeout Program**. I installed all the essential EDA tools and verified that they are working correctly. It was a long day, but now my system is ready for RTL design and SoC development.

---

## 📌 My System Configuration

- **OS:** Ubuntu 22.04 (VirtualBox VM)  
- **RAM:** 16 GB  
- **CPU:** 16 vCPU  
- **HDD:** 100 GB  

I checked that all the system requirements were met before starting the installations.

---

## 🛠 Tools I Installed

### 1. Yosys (RTL Synthesis)
I cloned the Yosys repository and installed all dependencies. Compiling took some time (~15 minutes), but the build finished successfully.  
**Verification:**  <img width="782" height="484" alt="yosys_img" src="https://github.com/user-attachments/assets/e925d101-0955-412f-ae69-c20b09bfa117" />

bash
yosys -V
Result: Yosys ran perfectly and showed version 0.34 (as expected).
✅ Ready for RTL synthesis tasks.

### 2. Icarus Verilog (iverilog)
I installed Icarus Verilog via apt-get. Installation was quick and smooth.
Verification:<img width="782" height="572" alt="image" src="https://github.com/user-attachments/assets/4a4dc3ff-a418-40c9-bfb8-f09ab5087e8f" />


bash
Copy code
iverilog -V
Result: Iverilog responded with the correct version.
✅ I can now simulate Verilog designs.

### 3. GTKWave (Waveform Viewer)
GTKWave was installed successfully with apt. I opened a test waveform to check that it works.
Verification:<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8b9b8597-bfed-49f8-aefd-927425e421e6" />
<img width="783" height="139" alt="image" src="https://github.com/user-attachments/assets/ef2da4ad-003a-40b3-bcf7-376a7d9a614a" />


bash
Copy code
gtkwave --version
Result: GTKWave launched and displayed the version info.
✅ Ready for waveform viewing.


✅ My Personal Observations
Yosys compilation took the longest, but I learned how dependencies affect building open-source EDA tools.

Docker setup was tricky at first, but adding my user to the group solved it.

Every tool was tested and verified with version checks and basic test commands.

Screenshots were taken for each tool to keep a record of successful installation.

I feel confident that my environment is fully prepared for the upcoming weeks of the program.
