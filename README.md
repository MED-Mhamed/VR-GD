# VR-GD: Virtual Reality Gestures Dataset With Leap Motion Controller

**Authors:**  Mohamed Mhamed , Anouar Ben Khalifa
**Contact:** [anouar.benkhalifa@eniso.u-sousse.tn](mailto:anouar.benkhalifa@eniso.u-sousse.tn)  
**License:** Publicly available for **non-commercial use**

---

## A. Description

The **VR-GD (Virtual Reality Gestures Dataset)** is a large-scale collection of **27,600 hand gesture samples** recorded from **30 participants** using a **head-mounted Leap Motion Controller (LMC)**.

It includes:
- **46 gestures**
- **41 dynamic gestures**
- **30 bimanual gestures**

VR-GD addresses the lack of bimanual and complex dynamic gestures in existing datasets. It captures realistic variations in hand size, skin tone, and facial structure, making it an ideal benchmark for **VR gesture recognition**, **HCI**, and **controller-free interaction research**.

![Dataset Overview]([images/dataset_overview.png](https://drive.google.com/file/d/12qRebIzjKSDl60t_S3Ap2Fym0JB8UO9Q/view?usp=drive_link))

## B. Dataset Format

We implemented a sophisticated data storage solution ensuring optimal management and acces- sibility. The directory structure follows a meticulous organizational approach:

Participant-specific directories: P{participant_id}

└──Gesture-specific subdirectories: G{gesture_num}

   └──Recording session subdirectories: R{recording_num}
   
---
![Dataset Format](images/dataset_overview.png)

The dataset’s technical architecture consists of two primary components:
Image Repositories (DEPTH DATA):
-Captured from left and right Leap Motion Controller cameras 
-Stored as grayscale .png files
-Consistent resolution: 240×640 pixels
-Separate ’left’ and ’right’ subdirectories maintaining camera-specific data integrity
Gesture Data Files (SKELETON DATA):
-Each recording session generates a detailed text file (hand_data_{timestamp}.txt)
-Captures: Frame ID, Timestamp, Hand detection confidence, Grip metrics, Arm and palm positioning, Detailed finger joint data


The VR-GD dataset transcends traditional data collection methodologies by establishing a foundational resource for advanced gesture recognition research. By providing a rich, multi- dimensional repository of hand movement data, this dataset not only supports intricate biomechanical analysis but also reveals new perspectives on human-machine interaction in immersive
environments

## C. Dataset Categorization 

Our novel dataset is evenly divided into four primary classes, each covering various aspects of VR system control and user interaction styles. This categorization ensures comprehensive exploration of VR interaction scenarios while providing a seeming functional distinction among gesture categories.
### 1. VR Mode Activation  
**Static (G1–G5)** — One- and two-hand gestures for system activation.

This category covers static gestures for quick VR mode activation and system boot. It comprises five simple static gestures performed with one hand (G1,G2,G3) and two hands (G4,G5). The gestures are designed for rapid recognition and serve as entry points to various VR interaction modes. Each gesture is characterized by a stationary hand shape that can be briefly held, limiting false positives and guaranteeing strong detection across users and contexts. 

**Sample Images:**  
![Activation 1](images/vr_mode_activation/G1.png)  
![Activation 2](images/vr_mode_activation/G2.png)  
![Activation 3](images/vr_mode_activation/G3.png)  
![Activation 4](images/vr_mode_activation/G4.png)  
![Activation 5](images/vr_mode_activation/G5.png)

**Video:**  
[Video Link](videos/vr_mode_activation.mp4)

---

### 2. Virtual Environment Navigation  
**Dynamic One-Hand Gestures (G6–G18)**
There are 13 dynamic one-hand gestures within the interaction space of the motion capture system. They include rotation, finger manipulation, and spatial trajectories for precise virtual environment navigation. They are characterized by temporal features and motion complexity with participants issuing gestures at various velocities.

**Sample Images (12):**  
![Navigation](images/navigation/G6.png)
![Navigation](images/navigation/G7.png)
![Navigation](images/navigation/G8.png)
![Navigation](images/navigation/G9.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)
![Navigation](images/navigation/G.png)

**Video:**  
[Video Link](videos/navigation.mp4)

---

### 3. Automotive VR Control  
**Dynamic Two-Hand Gestures (G19–G30)**

This category has 12 dynamic gestures performed using both hands, targeted at automotive VR purposes. These gestures are imitations of real driving interactions and car control devices, which are modeled upon bimanual coordinated hand movements.


**Sample Images (12):**  
![Automotive](images/automotive/G19.png)
![Automotive](images/automotive/G20.png)
![Automotive](images/automotive/G21.png)
![Automotive](images/automotive/G22.png)
![Automotive](images/automotive/G23.png)
![Automotive](images/automotive/G24.png)
![Automotive](images/automotive/G25.png)
![Automotive](images/automotive/G26.png)
![Automotive](images/automotive/G27.png)
![Automotive](images/automotive/G28.png)
![Automotive](images/automotive/G29.png)
![Automotive](images/automotive/G30.png)


**Video:**  
[Video Link](videos/automotive.mp4)

---

### 4. Gaming VR Environment  
**Advanced Bimanual Dynamic Gestures (G31–G46)**

This category has 16 advanced dynamic gestures performed using both hands, designed for interactive gaming VR environments. These gestures comprise intricate movement patterns, multi-step transitions, and coordinated bimanual actions.


**Sample Images (16):**  
![Gaming](images/gaming/G31.png)
![Gaming](images/gaming/G32.png)
![Gaming](images/gaming/G33.png)
![Gaming](images/gaming/G34.png)
![Gaming](images/gaming/G35.png)
![Gaming](images/gaming/G36.png)
![Gaming](images/gaming/G37.png)
![Gaming](images/gaming/G38.png)
![Gaming](images/gaming/G39.png)
![Gaming](images/gaming/G40.png)
![Gaming](images/gaming/G41.png)
![Gaming](images/gaming/G42.png)
![Gaming](images/gaming/G43.png)
![Gaming](images/gaming/G44.png)
![Gaming](images/gaming/G45.png)
![Gaming](images/gaming/G46.png)

**Video:**  
[Video Link](videos/gaming.mp4)

---
## F. Accessing the Dataset

The VR-GD dataset is **publicly available for non-commercial use**.

📩 **To request access, contact:**  
**anouar.benkhalifa@eniso.u-sousse.tn**

---

## G. Citation

If you use the VR-GD dataset, please cite:

```bibtex
@dataset{VRGD2025,
  title={VR-GD: Virtual Reality Gestures Dataset},
  author={ M. Mhamed, H. Chtioui, N. M. Bhiri, R. Amri, B. Seddik, and A. B. Khalifa},
  year={2025},
  institution={ENISo, University of Sousse},
  note={Available for non-commercial research use}
}
