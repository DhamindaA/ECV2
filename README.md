# ECV2: Eclipse Plugin for Corroborative Verification and Validation for Autonomous Systems

## 📘 Overview

This plugin supports corroborative verification and validation (V&V) workflow for an autonomous system. 

---

## 🛠 Prerequisites

Before installing, ensure you have:

- **Java 17 or newer** (recommended: Java 21)  
  Check with: `java -version`
- **Eclipse IDE for RCP and RAP Developers 2025-03 (4.35.0)** or newer  
  [Download Eclipse RCP/RAP Developer Edition](https://www.eclipse.org/downloads/packages/release/2025-03/r/eclipse-ide-rcp-and-rap-developers)

> ⚠️ *The RCP/RAP Developer edition includes the Plug-in Development Environment (PDE), which is required to install Eclipse plugins.*

---

## ⬇️ Download & Install

### 1. Get the Update Site ZIP

- Visit the [GitHub Release Page](https://github.com/DhamindaA/ecv2-eclipse-plugin/releases/tag/v1.0.0)
- Download: `ecv2-updatesite.zip`
- Save it anywhere on your computer

### 2. Unzip the File

Unzip the archive. You should see a folder containing:

- `artifacts.jar`  
- `content.jar`  
- `features/`  
- `plugins/`  
- `site.xml`  

> This is your Eclipse update site folder.

### 3. Install into Eclipse

1. Launch Eclipse IDE for RCP and RAP Developers  
2. Go to: `Help > Install New Software...`  
3. Click **Add...**  
4. In the dialog:
   - **Name**: `Corroborative Verification`
   - **Location**: Click **Local...** and browse to the unzipped folder  
5. Click **OK**  
6. Eclipse will scan and list: `ECV2Plugin Feature`  
7. Check the box next to the feature  
8. Click **Next**, then **Next** again  
9. Accept the license and click **Finish**  
10. Restart Eclipse when prompted  

✅ *The plugin is now installed.*

---

## ✅ Verifying Installation

After Eclipse restarts:

- Go to `Help > About Eclipse IDE > Installation Details`
- Confirm `ECV2Plugin.Feature` is listed

To launch the main view:

- Go to `Window > Show View > Other...`  
- Look for **Cross-Evidence Comparison**

---

## 🚀 Using the Plugin

### Linking Thresholds and Ontology URIs

1. Download [resources.zip](https://github.com/DhamindaA/ecv2-eclipse-plugin/blob/main/Resources.zip)  
   (contains `thresholds.json` and `ontology.json` to test the plugin)
2. Extract and save the files anywhere
3. In Eclipse:
   - Go to: `Window > Preferences > Corroborative V&V Resources`
4. Browse and select the folder containing the json files (e.g., `C:\Users\username\resources`)
5. Click **Apply and Close**

### Importing Evidence

1. Download [evidence.zip](https://github.com/DhamindaA/ecv2-eclipse-plugin/blob/main/Evidence.zip)  
   (contains `FormalModelChecking.json` and `ROS_Simulation.json` to test the plugin)
2. In Eclipse, go to the `Verification` menu  
3. Select `Import Evidence…`

### Viewing Cross-Evidence Comparison

After importing evidence, use the **Cross-Evidence Comparison** view to analyse discrepancies across different verification methods.

---

## ❌ Uninstalling the Plugin

To remove the plugin:

1. Go to: `Help > About Eclipse IDE > Installation Details`
2. Locate **ECV2Plugin Feature**
3. Select it and click **Uninstall**
4. Restart Eclipse when prompted

---

## 🧩 Troubleshooting

### Nothing shows in "Install New Software" dialog?

- Make sure you selected the **unzipped** update site folder, not the ZIP file
- Folder must contain:  
  `artifacts.jar`, `content.jar`, `features/`, `plugins/`, `site.xml`

### Error: "Cannot satisfy dependency"

- Ensure Eclipse version is **2025-03 (4.35.0)** or newer
- Java version must be **17 or newer** (recommended: Java 21)

### Plugin doesn't appear after installation

- Restart Eclipse
- Check `About > Installation Details` to verify it was installed

---

## 📩 Support

For questions or help, please contact:  
**Dhaminda Abeywickrama**  
📧 Dhaminda.Abeywickrama@manchester.ac.uk

---

## 📄 License

The ECV2 plugin binary is provided for academic and research use only. 
Redistribution, modification, or commercial use is not permitted without prior written permission from the author.
