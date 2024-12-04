
# Hand Gesture Recognition for Light Control

This project implements a hand gesture recognition system to control light simulations. It uses image processing and machine learning techniques to detect and interpret gestures for controlling light states. Below is the file structure and explanation for each component.

## Project Structure

The repository is organized into the following directories and files:

```
models/
│
├── sign_imgs2/
│   └── Step_0/
│       ├── data2/
│       ├── sign_imgs2/
│       └── generate_landmark_data.py
│       └── hand_gesture.yaml
│
├── Step_1/
│   ├── data/
│   ├── hand_gesture.yaml
│   └── Model_training.ipynb
│
├── Step_2/
│   ├── __pycache__/
│   ├── detect_simulation.py
│   ├── hand_gesture.yaml
│   └── requirements.txt
```

### 1. `sign_imgs2/Step_0/`
This is the first step of the pipeline, which includes:
- **`generate_landmark_data.py`**: Script for preprocessing and extracting hand landmarks from gesture images.
- **`hand_gesture.yaml`**: Configuration file defining parameters for the hand gesture data collection.

### 2. `Step_1/`
This step focuses on training the machine learning model:
- **`data/`**: Directory containing processed gesture data.
- **`Model_training.ipynb`**: Jupyter notebook for training the gesture recognition model.
- **`hand_gesture.yaml`**: Configuration file for model training, specifying parameters like hyperparameters, input formats, and data preprocessing steps.

### 3. `Step_2/`
This is the final step, focusing on deployment and simulation:
- **`detect_simulation.py`**: Script for running the trained model to detect hand gestures and control the light simulation.
- **`requirements.txt`**: Dependencies and libraries needed to run the simulation and detection scripts.
- **`hand_gesture.yaml`**: Configuration file for the simulation step.

---

## Prerequisites

To set up the environment, ensure you have the following installed:
- Python 3.8 or later
- Libraries listed in `requirements.txt`

Install the dependencies with:

```bash
pip install -r requirements.txt
```

---

## Usage

### Step 0: Generate Landmark Data
Run the `generate_landmark_data.py` script to extract landmarks from the hand gesture dataset:

```bash
python Step_0/generate_landmark_data.py
```

### Step 1: Train the Model
Use the `Model_training.ipynb` notebook to train the hand gesture recognition model. Load the notebook and execute the cells step-by-step.

### Step 2: Simulate and Detect Gestures
Run the `detect_simulation.py` script to test the system and simulate light control based on hand gestures:

```bash
python Step_2/detect_simulation.py
```

---

## Future Improvements
The system can be extended to include:
- Additional gestures for more control functionalities.
- Real-time video feed integration for dynamic gesture recognition.
- Improved accuracy through advanced models like convolutional neural networks.

---

## License

This project is licensed under the MIT License. See `LICENSE` for details.

---

## Acknowledgments

The project is inspired by the need for contactless control solutions and utilizes machine learning and computer vision techniques to achieve gesture-based control. Special thanks to all contributors and sources referenced in the project.

--- 
