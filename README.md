# 🛩️ Robust and Agile Quadrotor Flight via Adaptive Unwinding-Free Quaternion Sliding Mode Control

This repository provides the official code implementation for the manuscript:

**"Robust and Agile Quadrotor Flight via Adaptive Unwinding-Free Quaternion Sliding Mode Control"**  
*Amin Yazdanshenas and Reza Faieghi*  
[[📄 Paper (PDF)]](./Robust_and_Agile_Quadrotor_Flight_via_Adaptive_Unwinding-Free_Quaternion_Sliding_Mode_Control.pdf) • [[🎥 Video Demo]](https://youtu.be/yhFYXKonTRk)

We propose an adaptive quaternion-based sliding mode controller (AQSMC) for nano quadrotors that:
- Resolves the **unwinding issue** in quaternion-based controllers,
- Incorporates **adaptive switching gains** to handle unknown disturbances without overgrowth,
- Ensures **robust and agile flight** under limited onboard computation,
- Runs reliably on resource-constrained platforms like the Crazyflie 2.1.

We implement and test multiple quaternion-based sliding mode controllers, including **QSMC** and **AQSMC**, and compare them against widely used benchmark controllers such as:
- **GTC** – Geometric Tracking Controller,
- **ESMC** – Euler-based Sliding Mode Control,
- **QPD** – Quaternion PD for attitude + SMC for position.

Extensive hardware experiments were conducted, including:
- **3-DOF gimbal tests** for isolated attitude control,
- **Lemniscate trajectory tracking** in 6-DOF free flight,
- **Throw-launch recovery** from inverted initial conditions,
- **Wind disturbance rejection**, and
- **Sensitivity analysis** across different controller tunings and scenarios.

All results demonstrate superior performance, agility, and robustness of AQSMC over the benchmark methods.
---

## 📁 Repository Structure

```bash
CrazyAQSMC/
├── crazyflie-firmware/        # Modified Crazyflie firmware with out-of-tree controllers
├── crazyflie-lib-python/      # Python scripts to log, launch, and visualize experiments
├── Robust_and_Agile_Quadrotor_Flight_via_Adaptive_Unwinding-Free_Quaternion_Sliding_Mode_Control.pdf   # Paper PDF
