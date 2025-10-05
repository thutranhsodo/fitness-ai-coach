# Real-Time Fitness Exercise Classification and Counting from Video Frames

## Dataset:
- Dataset “InfiniteRep”, including 1000 videos, 10 popular exercises, 7 different contexts (living room, gym,...) with diverse lighting, angles, ...
- Focus on four exercises: Squat, Push-up, Barbell Bicep Curl, Shoulder Press

## Project Structure
- `main.py`: Runs the Streamlit app.
- `ExerciseAiTrainer.py`: Contains exercise-specific pose estimation logic.
- `AiTrainer_utils.py`: Utility functions for image processing and distance calculations.
- `PoseModule2.py`: Handles body pose estimation using MediaPipe.
- `requirements.txt`: List of required Python libraries.
- `syn_pose_data/`:  Synthetic pose data for training/evaluation
- `video_demo/`: Sample video showing proper form for exercises.
- `model/`: Pre-trained models for label encoding and feature scaling (for the model "Long Short Term Memory").

## Result
- Long Short-Term Memory:
<img width="574" height="227" alt="image" src="https://github.com/user-attachments/assets/772fc54a-34c7-44b9-8d3f-c3efcf0c2744" />

- Bidirectional LSTM:
<img width="574" height="227" alt="image" src="https://github.com/user-attachments/assets/ca5a01c0-1bcb-4f7a-b529-eaea7fe11c85" />

- Vision Transformer:
<img width="574" height="227" alt="image" src="https://github.com/user-attachments/assets/c8ffb7a4-65dc-43d5-8a08-d2b23afa6c97" />


## Installation
1. Clone the repository:  
git clone https://github.com/yourusername/FitnessAICoach.git  
cd FitnessAICoach  
2. Set up a virtual environment:  
python -m venv venv  
venv\Scripts\activate  
4. Install the required Python libraries:  
pip install -r requirements.txt  
5. Run the app:  
streamlit run main.py

## Overview of the WebApp
The Fitness AI Coach is an interactive web-based platform developed with Streamlit, designed to help users monitor their workouts through real-time exercise recognition, automatic repetition counting, and an integrated AI fitness assistant.  
From the sidebar menu, users can easily explore the main features of the app:
- Video Analysis: Upload pre-recorded workout videos to detect poses and automatically count repetitions.
- Webcam Mode: Perform exercises live in front of your camera for instant feedback and repetition tracking.
- Auto Classify Mode: The system automatically recognizes different exercise types in real time and counts reps accordingly.  

The application emphasizes a modular and intuitive design, featuring visual indicators and tutorial clips to guide users in maintaining proper exercise form and tracking performance effectively.

### Acknowledgment
This project is originally developed by [Riccardo Riccio](https://github.com/RiccardoRiccio/Fitness-AI-Trainer-With-Automatic-Exercise-Recognition-and-Counting).  
All credits for the original implementation go to the author.  
This repository is a personal fork used for study and experimentation purposes.
