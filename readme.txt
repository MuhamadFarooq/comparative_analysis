This project has different users data while watching 360-degree video. This data contains pitch and yaw angles which are recorded using HMD device. Roll angle is kept as 0 for this project.
Pitch and yaw angles are converted into pixel coordinates and plotted them on video width and height to see where they exist on video frame. 
Viewport size is kept as (1080, 1920) and video is of 8K resolution.
Using sequences of data for LSTM model input and sequence length is kept as 30.

Viewport predictions were done for next frame, 1, 2, 3, 5 and 8 seconds. For next frame viewport prediction, MLP model gives better accuracy (99%) while LSTM accuracy is 93.57%.
For long-term predictions, LSTM perfoms better than other ML models, also sequential models (LSTM, GRU, RNN) have better performance in terms of accuracy than non-sequential models (LR, MLP).
