# Virtual Mouse: A Gesture-Based Interface

**Project Background:** This repository contains a legacy project demonstrating hand tracking as a mechanism for computer interaction. While developed earlier in my learning journey, it offers a functional illustration of computer vision techniques applied to create a gesture-controlled virtual mouse. 

### Project Overview:

This project enables hands-free cursor control and click actions through a computer's webcam. Utilizing real-time video analysis, hand movements are translated into mouse inputs, providing a unique and intuitive interaction method. 

### Technical Approach:

The system leverages two Python modules:

1. **`htm.py` (Hand Tracking Module):**
   * Implements hand detection and landmark identification using the MediaPipe library. 
   * Supplies real-time data on hand posture, including finger positions.

2. **`virtualmouse.py` (Application Script):**
   * Receives hand-tracking data from `htm.py`. 
   * Maps user gestures to corresponding mouse events. Specifically, index finger movement directs the cursor, while pinching the index and middle fingers together triggers a click.
   * Employs the `pyautogui` library for system-level simulation of mouse actions. 

### Considerations and Future Directions:

* **Lighting:** Performance is affected by lighting conditions. Incorporating techniques like adaptive thresholding or integrating depth-sensing cameras could improve robustness.
* **Expanded Gesture Set:**  Currently, only basic cursor control and left-clicking are supported. The addition of more gestures (e.g., scrolling, right-click, etc.) would enhance usability. 
* **Responsiveness:** Potential exists to refine smoothing algorithms or address latency to further optimize response time.  

**The codebase is open for experimentation and improvement.** Please feel free to explore its functionality and contribute.
