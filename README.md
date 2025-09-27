# seeVieweR 🧠🔍  
*A fast, interactive MATLAB App for neuroimaging visualization*  

**seeVieweR** is a MATLAB App Designer tool for interactive exploration of 3-D and 4-D neuroimaging data.  
It supports **volume rendering, overlays, masks, erosion, slice controls, and high-quality export** — all from a clean and responsive interface.  

## 🎬 Demo (animated)  
*(Replace this placeholder with your own `.gif` demo)*  

![seeVieweR Demo](docs/inflow_post.gif)  

## ✨ Features
- **High-quality 3-D/4-D visualization**  
  Built on `viewer3d` + `volshow` with a single persistent instance for fast updates.  

- **Overlay support**  
  Load multiple overlays with independent colormaps, thresholds, alpha transparency, and saved states.  

- **Interactive controls**  
  - Intensity and threshold sliders  
  - Slice masks (X/Y/Z)  
  - Vessel erosion with skeleton protection  
  - Adjustable opacity and contrast ramps  

- **Custom colormaps & histograms**  
  Compact colorbar panels with inline histograms (percentile-clipped & sqrt-scaled).  

- **Masking**  
  - Brain masks  
  - ROI/territory masks  
  - Slice masks  

- **Export & reproducibility**  
  - PNG snapshots with colorbars  
  - Quick slice mosaics in any orientation  
  - Animated GIF/MP4 movie export (time series or rotating camera)  
  - Full state save/load for reproducible visualization  

## 🚀 Installation
1. Download the latest **`seeVieweR.mlappinstall`** release from this repository.  
2. Double-click the file, or in MATLAB use:  

   matlab.apputil.install('seeVieweR.mlappinstall')
3. Once installed, seeVieweR will appear in the Apps toolbar - Launch it anytime from there — no need to add paths manually.

## 📋 Quick Reference

| Control | Function |
|---------|----------|
| **Base/Overlay Slider** | Set display intensity range. |
| **Threshold Sliders** | Hide voxels outside range (base/overlay). |
| **ORI1/ORI2/ORI3** | Slice masks in X/Y/Z. |
| **Base Alpha Spinner** | Base volume opacity. |
| **Overlay Alpha Spinner** | Overlay opacity. |
| **Contrast Spinner** | Adjust base contrast (gamma warp). |
| **Flip Map Switch** | Invert colormap (base/overlay). |
| **Lighting Switch** | Toggle lighting on/off. |
| **Denoising Switch** | Toggle denoising filter. |
| **Colormap Dropdowns** | Choose base/overlay colormap. |
| **Rendering Dropdown** | Select rendering style (volume, MIP, etc.). |
| **Background Dropdown** | Set background color. |
| **Territory Dropdown** | Apply vascular territory masks. |
| **Erosion Controls** | Vessel erosion with skeleton protection. |
| **Export Frame** | PNG + colorbars. |
| **Quick Plot** | Slice mosaics. |
| **Export Movie** | Animated GIF/MP4. |
| **Save/Load State** | Full restoration of viewer settings. |

## 📦 Requirements
- MATLAB R2023b or later (R2024a+ recommended).  
- Image Processing Toolbox.  
- Statistics & Machine Learning Toolbox (for some functions).  
- Optional: [`brewermap`](https://nl.mathworks.com/matlabcentral/fileexchange/45208-cbrew-brewer-colormaps) / [`crameri`](https://www.mathworks.com/matlabcentral/fileexchange/52398-crameri-perceptually-uniform-colormaps) colormap toolboxes.  

## 📖 License
Distributed under the GNU GPL v3 (or later). See `LICENSE` for details.  

