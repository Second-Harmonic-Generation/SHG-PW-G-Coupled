## 🧰 How to Use This Template    

Click the green **"Use this template"** button at the top of the page, then choose **"Create a new repository"**.   

This will create your own copy of this project, which you can modify freely — no need to fork!   

 
<p align="center">
  <img src="./images/SHG-banner.png" alt="SHG Logo">
</p>


<h1 align="center">SHG-PW-G-Heat-Equation</h1>

<div align="center">

| **Term** | **Definition** |
|----------|----------------|
| **SHG** | Second Harmonic Generation |
| **PW** | Pulsed Wave |
| **G** | Gaussian |
</div>

&nbsp;

<div align="center">

Article title:       
**Complete Anisotropic Time-Dependent Heat Equation in KTP Crystal under Repetitively Pulsed Gaussian Beams: A Numerical Approach**
</div>

&nbsp;

---

***Table of Contents***

<div>
  &nbsp;&nbsp;&nbsp;&nbsp;<a href="#1-about-this-repository"><i><b>1. About this repository</b></i></a>
</div>
&nbsp;

<div>
  &nbsp;&nbsp;&nbsp;&nbsp;<a href="#2-getting-started"><i><b>2. Getting Started</b></i></a>
</div>
&nbsp;

<div>
  &nbsp;&nbsp;&nbsp;&nbsp;<a href="#3-how-to-cite-us"><i><b>3. How to Cite Us</b></i></a>
</div>
&nbsp;


<div>
  &nbsp;&nbsp;&nbsp;&nbsp;<a href="#4-contact-information"><i><b>4. Contact Information</b></i></a>
</div>
&nbsp;

---    

## 1. About this repository


This repository contains the **toolkit and computational tools** used in the research article **"Complete Anisotropic Time-Dependent Heat Equation in KTP Crystal under Repetitively Pulsed Gaussian Beams: A Numerical Approach"** (Applied Optics, 2015), including source code, numerical solvers, and reproducibility assets.  


This toolkit provides computational tools for analyzing **transient temperature distribution** in cylindrical nonlinear potassium titanyl phosphate (KTP) crystals under repetitively pulsed Gaussian pumping sources. The toolkit implements a thorough and detailed solution for the time-dependent heat equation using advanced modeling features that are often neglected in simpler approaches:  

- **Temperature-dependent thermal conductivity** of KTP crystal  
- **Convective and radiative boundary conditions** at crystal surfaces  
- **Finite Difference Method (FDM)** for numerical calculations  

The research demonstrates that the radiation term has a negligible effect and can be safely ignored, while the temperature dependence of thermal conductivity is more influential. Ignoring temperature-dependent thermal conductivity introduces significant errors into the modeling. The toolkit shows the time evolution of temperature as the crystal is pumped with a train of successive Gaussian pulses until reaching thermal equilibrium. These tools improve modeling accuracy for **thermal lensing, phase mismatching, and efficiency reduction** in nonlinear optical systems, particularly in second harmonic generation applications.  


```
Folder PATH listing
+---citation                      <-- Contains citation materials and papers
│       1_Heat-Equation_Continu…  <-- Heat equation analytical paper
│       2_Heat-Equation_Continu…  <-- Heat equation continuous wave paper
│       3_Heat-Equation_Pulsed-…  <-- Heat equation pulsed wave paper
│       4_Phase-Mismatch_Pulsed…  <-- Phase mismatch pulsed wave paper
│       5_Ideal_Continuous-Wave…  <-- Ideal continuous wave paper
│       6_Ideal_Pulsed-Wave_Be…   <-- Ideal pulsed wave Bessel paper
│       7_Coupled_Continuous-Wa…  <-- Coupled continuous wave paper
│       README.md                 <-- Citation guidelines and information
│
+---images                        <-- Contains project images and logos
│       SHG-banner.png            <-- SHG project banner
│
+---results                       <-- Numerical simulation results
│       E_009_f_500_Np_10_tp_50…  <-- Thermal conductivity radial data
│       E_009_f_500_Np_10_tp_50…  <-- Thermal conductivity transverse data
│       E_009_f_500_Np_10_tp_50…  <-- Thermal conductivity axial data
│       E_009_f_500_Np_10_tp_50…  <-- Temperature radial data
│       E_009_f_500_Np_10_tp_50…  <-- Temperature transverse data
│       E_009_f_500_Np_10_tp_50…  <-- Temperature axial data
│
+---src                           <-- Contains source code
│       Code_SHG_PW_G_Heat-Equ…   <-- Fortran finite difference solver
│
│       Article_SHG-PW-G-Heat-…   <-- Main research paper PDF
│       CITATION.cff              <-- Citation metadata file
│       LICENSE                   <-- Project license information
│       README.md                 <-- Project overview and documentation
│

```

## 2. Getting Started

### 2.1. Prerequisites

To run this project, you will need the following software and tools:

- **Fortran Compiler** (gfortran, Intel Fortran, or similar)
  - For Ubuntu/Debian: `sudo apt-get install gfortran`
  - For macOS: `brew install gfortran`
  - For Windows: Install MinGW-w64 or Intel Fortran Compiler
- **Git** (for cloning the repository)
- **Text Editor or IDE** (VS Code, Cursor, or any Fortran-compatible editor)
- **Terminal/Command Line Interface**

### 2.2. Quick Start

Follow these steps to get the project running:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/SHG-PW-G-Heat-Equation.git
   cd SHG-PW-G-Heat-Equation
   ```

2. **Navigate to Source Directory**
   ```bash
   cd src
   ```

3. **Compile the Fortran Code**
   ```bash
   gfortran -o heat_equation_solver Code_SHG_PW_G_Heat-Equation.f90
   ```

4. **Run the Simulation**
   ```bash
   ./heat_equation_solver
   ```

5. **View Results**
   - The program will generate output files in the `results/` directory
   - These files contain temperature distribution data and thermal conductivity data
   - You can analyze the results using your preferred data analysis tools

6. **Optional: Development Environment**
   - Open the project in VS Code or Cursor for better code editing experience
   - Install Fortran language extensions for syntax highlighting and debugging
   - Use the integrated terminal for compilation and execution

**Note**: The simulation parameters can be modified directly in the Fortran source code (`Code_SHG_PW_G_Heat-Equation.f90`) to explore different scenarios and crystal configurations.


## 3. How to Cite Us
Please refer to the [**citation**](./citation/) folder for accurate citations. It contains essential guidelines for accurate referencing, ensuring accurate acknowledgement of our work.

  
## 4. Contact Information

For questions not addressed in the resources above, please connect with [Mostafa Rezaee](https://www.linkedin.com/in/mostafa-rezaee/) on LinkedIn for personalized assistance.
