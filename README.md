# Universal Bootstrap Calculator

A compact and universal tool for calculating bootstrap component requirements used in high‑side MOSFET driver circuits.

This calculator determines:
- Total required charge (Qtotal)
- Maximum allowed voltage drop (ΔVHB)
- Minimum bootstrap capacitor (Cboot)
- Recommended VDD supply capacitor (CVDD ≥ 10 × Cboot)
- RC time constant (τ)
- Peak diode inrush current
- Stored energy in Cboot

The tool is universal and **not tied to any specific manufacturer**.  
It uses standard bootstrap equations to ensure compatibility with any high‑side MOSFET driver topology.

---

## ✅ Features

- Clean and compact graphical interface (PyQt6)
- Color‑coded input categories:
  - **Blue:** MOSFET parameters  
  - **Green:** Driver parameters  
  - **Orange:** Diode parameters  
  - **Grey:** User‑chosen elements  
- Interactive tooltips (ⓘ) explaining each parameter
- Scrollable results panel
- Automatic computation of all essential bootstrap quantities
- No external dependencies except Python 3 + PyQt6 (for the source version)

---

## ✅ Download (.exe)

You can download the Windows executable from the **Releases** section:

👉https://github.com/Hsannriahi/Universal-bootstrap-calculator/releases/tag/v1.0.0
No installation is required.  
Just run the `.exe`.

---

## ✅ Usage Instructions

1. Enter the required parameters:
   - MOSFET gate charge (Qg)
   - Driver supply voltage (VDD)
   - Duty cycle (%)
   - Switching frequency (kHz)
   - Leakage and quiescent currents (IHBS, IHB)
   - Diode forward voltage (Vf)
   - UVLO falling threshold
   - Bootstrap resistor (Rboot)

2. Click **Calculate**  
3. The results panel will display:
   - Formulas  
   - Numerical values  
   - Recommended capacitor sizes  
   - All bootstrap design metrics


Install PyQt6:

```bash
pip install pyqt6
