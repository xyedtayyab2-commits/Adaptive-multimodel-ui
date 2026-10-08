# Adaptive Multimodal UI

## Introduction

This project combines three different Human-Computer Interaction concepts into one web-based interface:

* Speech interaction
* Gesture and touch interaction
* Eye-gaze interaction
* Adaptive user interface based on the input method

The main purpose of this project is to show how a user can interact with the same interface using different input methods. The interface also changes its behavior depending on whether the user is using a mouse, touch screen, or keyboard.

## Features

### 1. Speech Control

The project uses the browser's Web Speech API to recognize simple voice commands.

The user can say commands such as:

* **Red** – changes the box to red
* **Blue** – changes the box to blue
* **Green** – changes the box to green
* **Bigger** – increases the size of the box
* **Smaller** – returns the box to its normal size
* **Reset** – returns the box to its original position, color, and size

To use this feature, click the **Start Voice Control** button and allow microphone access if the browser asks for permission.

### 2. Gesture and Touch Interaction

The blue box can be moved around the stage using the mouse.

The user can:

* Click and drag the box with a mouse
* Drag the box using a touch screen
* Move the box within the boundaries of the stage

This demonstrates direct manipulation and gesture-based interaction.

### 3. Eye-Gaze Simulation

A real eye-tracking camera is not required for this project.

Instead, mouse movement is used to simulate the user's gaze.

When the mouse is moved over one of the cards, the system starts measuring the time spent over that card. If the mouse stays over a card for more than **500 milliseconds**, the card is considered fixated.

The selected card gets a visual highlight and the gaze pointer becomes larger.

The interface also displays:

* Current gaze position
* Current fixation target
* Dwell time

### 4. Adaptive UI

The interface automatically detects the type of input being used.

#### Mouse Mode

When the mouse is being used, the interface keeps the controls relatively compact for precise interaction.

#### Touch Mode

When a touch interaction is detected, the buttons become larger so they are easier to tap with a finger.

#### Keyboard Mode

When the user presses the **Tab** key, the interface switches to keyboard mode and provides a more visible focus indicator.

This demonstrates the idea of an adaptive interface that responds to the user's interaction modality.

## Technologies Used

The project was created using basic web technologies:

* **HTML5** – structure of the interface
* **CSS3** – styling and responsive/adaptive design
* **JavaScript** – interaction and functionality
* **Web Speech API** – speech recognition
* **Mouse Events** – gaze simulation and mouse interaction
* **Touch Events** – touch and gesture interaction
* **Keyboard Events** – keyboard modality detection

## How to Run

No server or installation is required.

1. Download the `adaptive_multimodal_ui.html` file.
2. Open the file in a modern web browser.
3. For speech control, allow microphone permission when requested.
4. Try dragging the box with the mouse or touch.
5. Move the mouse over the cards and keep it still for at least 500 ms to test eye-gaze fixation.
6. Press the **Tab** key to test keyboard adaptation.

For the best speech-recognition experience, use a browser that supports the Web Speech API, such as Google Chrome.

## Project Objective

The main objective of this project is to demonstrate how multiple interaction techniques can be combined into a single user interface.

Instead of creating separate interfaces for speech, gestures, eye tracking, and different input devices, this project brings them together and allows the interface to adapt according to how the user interacts with it.

## Conclusion

This project demonstrates a basic example of a multimodal and adaptive user interface. It combines voice commands, direct manipulation, touch gestures, simulated eye tracking, and automatic modality detection.

Although the eye-tracking feature uses the mouse as a simulation rather than a real eye-tracking device, it demonstrates the basic concept of fixation and dwell time that can be used in a real eye-tracking system.
