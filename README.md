#  Self-Driving Car AI (Vanilla JS)

A browser-based simulation of self-driving cars trained using a simple neural network and evolutionary principles — built **from scratch using pure JavaScript (no libraries)**.

---

## Overview

This project simulates multiple AI-controlled cars learning to drive on a multi-lane road while avoiding traffic.

Each car:

* Uses **virtual sensors** to detect surroundings
* Feeds data into a **neural network**
* Makes real-time driving decisions (forward, left, right, reverse)

Over time, the system evolves better drivers using **mutation and selection**.

---

##  How It Works

### 1. Sensors

* Rays are cast in multiple directions
* Detect distance to road borders and other cars
* Provide normalized input to the neural network

### 2. Neural Network

* Fully custom implementation (no frameworks)
* Architecture:
  `input layer → hidden layer → output layer`
* Example:

  ```
  [sensor inputs] → [6 neurons] → [4 outputs]
  ```

### 3. Outputs (Controls)

* Forward
* Left
* Right
* Reverse

The network decides these values every frame.

---

### 4. Evolution (Genetic Algorithm)

* Multiple cars are generated
* Best-performing car is selected (based on distance traveled)
* Its "brain" is saved and mutated to create new generations

---

## Features

* Built using **Vanilla JavaScript (no external libraries)**
*  Custom Neural Network implementation
*  Sensor-based environment awareness
*  Collision detection using polygons
*  Evolution via mutation
*  Save / Load best AI using `localStorage`
*  Real-time neural network visualization

---

##  Controls

* AI cars drive automatically
* Optional manual controls (if enabled in code)

---

##  How to Run

1. Clone the repository:

   ```
   git clone https://github.com/shriyaagg/self-driving-car-ai.git
   ```

2. Open the project folder

3. Run `index.html` in your browser

---

##  Tips

* Click **Save** to store the best AI or the best car
* Refresh the page to continue training
* Click **Discard** to reset learning

---

## Project Structure

```
/project-folder
│── index.html
│── style.css
│── main.js
│── car.js
│── sensor.js
│── network.js
│── controls.js
│── road.js
│── utils.js
│── visualizer.js
│── car.png
```

---




