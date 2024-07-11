# 📱 Mobile Nuclei Templates

This repository contains Nuclei templates designed for static analysis of Android applications. These templates help identify various security vulnerabilities and weaknesses by analyzing the source code and configuration files of the applications.

## 🚀 Getting Started

### Requirements

- `apktool`: A tool for decompiling and recompiling Android APK files.
- `nuclei`: A tool for fast and customizable vulnerability scanning based on templates.

### Installation

1. **Install Apktool**:
    ```sh
    sudo apt install apktool -y
    ```

2. **Install Nuclei**:
    Follow the instructions on the [Nuclei GitHub page](https://github.com/projectdiscovery/nuclei) to install Nuclei.

### Download Mobile Nuclei Templates

Clone the repository containing the Nuclei templates:
```sh
git clone https://github.com/YoruYagami/mobile-nuclei-templates.git
```

### Example Usage with AndroGoat

1. Decompile the AndroGoat APK file to extract its contents:
```sh
apktool d AndroGoat.apk
```

2. Use Nuclei to perform static analysis on the decompiled APK:
```sh
echo AndroGoat/ | nuclei -t mobile-nuclei-templates/
```

📋 Cheat Sheet
- Install Apktool: sudo apt install apktool
- Clone Templates: git clone https://github.com/YoruYagami/mobile-nuclei-templates.git
- Decompile APK: apktool d <your-app>.apk
- Run Nuclei Scan: echo <decompiled-app-path>/ | nuclei -t mobile-nuclei-templates/