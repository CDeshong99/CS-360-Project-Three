# Sensor Tracker App – Project Three
This mobile app was created as part of Project Three in the CS 360 Mobile Architecture course. It demonstrates how to design, develop, and test an Android application using SensorManager to read data from the device's built-in accelerometer.
# App Overview & Requirements
The primary goal of this app is to allow users to monitor real-time X, Y, and Z axis data using their device’s accelerometer. It addresses the need for a lightweight, privacy-focused sensor tool that can be used by students, developers, or anyone interested in motion data without unnecessary features or permissions.
# UI Design & Screens
The application features a single, clean screen with three TextView components showing live accelerometer values. The UI is user-centered: it's minimalistic, easy to read, and updates in real-time. We focused on a clutter-free design to ensure accessibility and ease of use.
Features:
Sensor monitoring using SensorManager

Real-time updates for X, Y, Z axis values

Accelerometer data automatically refreshes as the device moves

Responsive layout for a variety of screen sizes
# Coding Approach & Techniques
The app was written in Kotlin using Android Studio. The development focused on clean code, modular structure, and Android best practices. I used SensorEventListener for real-time tracking, and ensured sensor registration/unregistration in lifecycle methods (onResume/onPause). This approach could be reused for future sensor apps or expanded to support additional sensors like gyroscopes.
# Testing & Functionality
Testing was completed in the Android Emulator (API 34) and included:

Verifying real-time updates on simulated motion changes

Ensuring text views responded correctly to changes

Setting breakpoints to confirm values were updated and handled correctly

This process confirmed that the app worked as intended and revealed the importance of properly registering and unregistering sensors to avoid resource leaks.
# Development Process & Challenges
The full process included ideation, design planning, Kotlin implementation, UI linking, and emulator-based testing. One challenge was dynamically updating values smoothly and consistently. I solved this by using SensorManager.SENSOR_DELAY_NORMAL and limiting UI operations to essential updates only, which prevented UI lag.
# Skills Demonstrated
The component I was most proud of was the seamless integration of hardware-level sensor data into a simple UI. This required an understanding of Android lifecycle methods, permissions, and sensor management—all while maintaining performance and clarity. It was a strong demonstration of my ability to develop efficient, user-focused mobile apps.
