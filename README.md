<div align="center">

<img src="https://img.shields.io/badge/Python-QA%20Automation%20Scripts-3776ab?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Domain-Android%20%7C%20Camera%20%7C%20ADB-10b981?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Level-Senior%20QA%20Architect-f59e0b?style=for-the-badge"/>

# 🐍 VaniPython — QA Automation Scripts

### Python Utilities & Scripts for Android QA Automation

**ADB tools · Camera metrics · Memory profiling · Defect analysis scripts**

</div>

---

## 📌 What Is This?

A personal collection of Python scripts and utilities built during 17+ years of QA automation work at Samsung R&D Institute India. Covers Android ADB automation, camera quality metrics, memory leak detection, and test data processing.

---

## 📁 Scripts Overview

### 🔧 ADB Utilities
```
adb_device_monitor.py    → Monitor multiple devices, auto-reconnect on drop
adb_memory_tracker.py    → Track PSS/RSS memory over test iterations
adb_crash_parser.py      → Parse tombstone files, extract crash signatures
adb_logcat_filter.py     → Filter logcat by tag, priority, package name
```

### 📸 Camera Quality
```
ssim_calculator.py       → SSIM score between two images
psnr_calculator.py       → PSNR measurement for image fidelity
color_accuracy.py        → ΔE2000 color difference vs Macbeth chart
exif_reader.py           → Extract EXIF data (ISO, shutter, focal length)
```

### 🔍 Defect Analysis
```
defect_trend_analyzer.py → Sprint-wise defect trend visualization
duplicate_detector.py    → Find duplicate defects by NLP similarity
severity_classifier.py   → Auto-classify S1/S2/S3/S4 from description
```

### 📊 Test Data
```
test_data_generator.py   → Generate bulk test data (users, products, etc.)
csv_to_json.py           → Convert test data formats
fixture_builder.py       → Build pytest/Jest fixtures from Excel
```

---

## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/vanichalla24/vanipython.git
cd vanipython

# Install dependencies
pip install -r requirements.txt

# Run any script
python adb_memory_tracker.py --device emulator-5554 --package com.samsung.camera --iterations 20
```

---

## 🔑 Key Scripts

### Memory Leak Detector
```python
# Tracks PSS memory over N iterations
# Flags if growth > threshold (default 50MB)
python adb_memory_tracker.py \
  --device emulator-5554 \
  --package com.samsung.camera \
  --iterations 50 \
  --threshold 50
```

### SSIM Calculator
```python
# Compare two images for structural similarity
python ssim_calculator.py \
  --reference reference_image.jpg \
  --test captured_image.jpg
# Output: SSIM Score: 0.943 (PASS — threshold 0.90)
```

---

## 👩‍💻 Author

**Vaani Challa** — QA Architect | Samsung SRIB | 17+ Years
Android · Camera · ISP Pipeline · Python · ADB

---

## 📄 License

MIT © [Vaani Challa](https://github.com/vanichalla24)
