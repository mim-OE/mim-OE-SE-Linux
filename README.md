# mimOE-SE-Linux

**mimOE (mim Operating Environment)**, mimOE-SE-Linux Standard Edition for Ubuntu Linux, supports the following platforms and architectures:

1. **mimOE for Linux** on Intel and AMD for Ubuntu 22.04 and above releases.
   - **Note:** Intel/AMD CPUs require Advanced Vector Extensions 2 (AVX2) support.
2. **mimOE for Linux-ARM64** for Ubuntu 22.04.2 LTS and above releases on Raspberry Pi or NVIDIA Jetson, including Jetson Orin Nano/AGX.
3. **mimOE for Linux-ARM CUDA** for Ubuntu 22.04.2 LTS and above releases on NVIDIA Jetson (with CUDA support), including Jetson Orin Nano/AGX.
   **Note:** The CUDA-enabled edition `mimOE-SE-linux-developer-arm64-CUDA` binary is significantly larger in size due to the inclusion of NVIDIA CUDA components (`.nv_fatbin`).

### CPU Requirements for Intel/AMD Processors

CPU with Advanced Vector Extensions 2 (AVX2) support
* Intel
    * Haswell processors (Q2 2013) and newer, except models branded as Celeron and Pentium.
    * Celeron and Pentium branded processors starting with Tiger Lake (Q3 2020) and newer.
* AMD
    * Excavator processors (Q2 2015) and newer.

#### Compatibility Warning
Attempting to run this software on a Intel/AMD CPU without AVX2 support may result in "Illegal Instruction" errors or crashes.
Please ensure your system meets the minimum CPU requirements before installation.

## Before You Start
- [Explore developer resources & documentation](https://developer.mimik.com)
- [Sign up and create a mimik developer console account](https://developer.mimik.com/console/create_account)

## Installation Guide
1. Download the latest .tar files for the latest release [HERE](https://github.com/mimik-mimOE/mimOE-SE-Linux/releases).
2. Create a new directory.
3. Move the downloaded .tar file to the newly created directory.
4. Open a terminal and navigate to the directory containing the downloaded `.tar` file.
5. Untar the package using the following command, replacing `<downloaded mimOE tar file>` with the actual filename. For example, for X86-64 (AMD64) Linux Ubuntu:

   ```
   tar xvf mimOE-SE-linux-developer-AMD64-v3.12.0.tar
   ```

6. Run the start script to launch mimOE:

   ```
   ./start.sh
   ```

7. Visit the [Developer Console](https://developer.mimik.com/console/create_account) to create an account and get started with your projects.

## Notes:

- After extracting, a directory may be created. Navigate into this directory to find the `start.sh` script.
- Do not close the terminal window where mimOE is running. Closing this window will terminate the mimOE process.
- To stop mimOE, close the terminal or use the keyboard shortcut `CTRL + C` in the terminal where it is running.
