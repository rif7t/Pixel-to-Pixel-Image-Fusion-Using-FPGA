# Pixel-to-Pixel Image Fusion Using FPGA

![License](https://img.shields.io/badge/license-MIT-informational)

## 📌 Project Overview
This project implements **pixel-to-pixel image fusion** using FPGA logic.  
It combines two input image streams at the pixel level, enabling high-throughput or real-time image processing in hardware (VHDL).

**Key Features:**
- VHDL modules for image buffering, synchronization, and fusion logic
- FPGA project files for building & synthesis
- Test modules and example image data for validation
- Extensible architecture for advanced fusion techniques

---

## 🧩 Architecture Overview

- **Pixel-to-Pixel-Image-Fusion-Using-FPGA/**
  - **.github/** *(if any CI/CD workflows exist)*
  - **apps/** *(optional if you have simulation/test apps)*
  - **Divider_Circuit.vhd** – Example VHDL module
  - **base_interf.vhd** – Base interface definition
  - **fifo_new.\*** – FIFO modules
  - **fifoa.\*** – Additional FIFO instance
  - **fifob.\*** – Additional FIFO instance
  - **image1.\*** – Example input image module
  - **image2.\*** – Example input image module
  - **std_dev.txt** – Standard deviation test data
  - **std_dev.vhd** – VHDL logic for standard deviation
  - **sync_clk2.\*** – Clock synchronization modules
  - **vga_lab_1.vhd** – VGA output module
  - **window_3x3.\*** – 3x3 windowing logic modules
  - **GROUP REPORT.docx** – Project report/documentation
  - `README.md`


---

## ✅ Prerequisites
- FPGA development board compatible with the project files
- FPGA toolchain (e.g., Intel Quartus, Xilinx Vivado)
- Basic knowledge of VHDL and FPGA design flow
- Optional: image capture or interface logic for real-time testing

---

## 🚀 How to Build & Run
1. Open the FPGA project file (`3x3window.qpf`) in your FPGA design software
2. Set the target FPGA device, board settings, clock constraints, and I/O pins
3. Synthesize and implement the design
4. Generate the bitstream / programming file
5. Upload/program the bitstream to the FPGA board
6. Connect input image sources (test patterns or real sensors)
7. Monitor the fused output via VGA/HDMI or other interfaces
8. Use included example modules (`image1`, `image2`) for internal testing

---

## 📊 How It Works
- Input streams are buffered and synchronized using FIFO modules (`fifo_new`, `fifoa`, `fifob`)
- `window_3x3` generates a 3x3 pixel window for local neighborhood processing
- `std_dev.vhd` calculates standard deviation or other pixel statistics
- Fusion logic combines pixel values (e.g., averaging or high-contrast selection)
- Output is displayed via `vga_lab_1.vhd` for real-time observation

---

## 🔧 Extension Ideas
- Implement advanced fusion techniques (multispectral, wavelet-based, neural networks)
- Add memory buffering for full-frame processing
- Hardware-accelerated image pre-processing (filtering, contrast adjustment)
- Adapt design for higher resolution or frame rates
- Integrate external camera modules for a full capture-process-display pipeline

---

## 📝 License
This project is licensed under the MIT License – see the LICENSE file for details.

---

## 💬 Contact
Questions, suggestions, or collaborations?  
- GitHub: [rif7t](https://github.com/rif7t)  
- Issues / Pull Requests: Open on this repository
