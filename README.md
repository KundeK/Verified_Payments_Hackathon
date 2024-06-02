# Project README

## Project Overview

This project involves the design and implementation of a web extension for enhanced security during online payments. The extension features a unique user interaction model combined with a secondary verification system based on real-time facial recognition.

## Features

### 4-by-4 Image Grid Interaction

**Technologies Used:**
- JavaScript
- HTML
- CSS

**Functionality:**
- Creates a 4-by-4 grid of randomly generated images.
- Users must successfully drag and drop three correct images in succession to autofill their saved credit card information.
- Enhances security by requiring a specific user interaction pattern before auto-filling sensitive information.

### Secondary Payment Verification

**Technologies Used:**
- Python
- MediaPipe
- OpenCV

**Functionality:**
- Implements a real-time facial recognition system to verify user identity during the 4-by-4 grid interactions.
- Extracts eye blink and position data to confirm the user's identity based on their behavior.
- Ensures that the correct user is performing the drag-and-drop actions, adding an extra layer of security.

## Implementation Details

### Web Extension

1. **Setup:**
   - Use JavaScript, HTML, and CSS to build the web extension interface.
   - Create a 4-by-4 grid layout with images that are randomly generated each session.

2. **Drag and Drop Mechanism:**
   - Implement drag and drop functionality using JavaScript's event listeners.
   - Ensure that users must drag and drop the correct sequence of images to trigger the autofill of credit card information.

3. **Autofill Credit Card Information:**
   - On successful drag and drop of the correct images, autofill the user's saved credit card information into the payment form.

### Facial Recognition System

1. **Setup:**
   - Use Python's MediaPipe and OpenCV libraries to develop the facial recognition system.
   - Configure the system to run in real-time and capture facial features.

2. **Data Extraction:**
   - Extract eye blink and position data during user interactions with the 4-by-4 grid.
   - Use this data to perform behavioral-based identity confirmation.

3. **Verification Process:**
   - Continuously monitor and analyze facial data during grid interactions.
   - If the behavior matches the expected patterns, allow the autofill process to proceed.
   - If discrepancies are found, prompt the user for additional verification.

