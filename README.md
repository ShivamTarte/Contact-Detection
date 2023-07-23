# Player Contact Detection

## Introduction

Welcome to the "Player Contact Detection" project! This repository houses the code and resources utilized in my second Kaggle competition. The primary goal of this competition was to detect instances of player contact in numerous American football games, similar to rugby. The detection was based on various factors, including distance, acceleration, orientation, and other relevant metrics. The data used for this task was collected at a frequency of 10 Hz, providing a detailed and comprehensive dataset for analysis.

## Algorithm Overview

To tackle this problem, I developed an algorithm that incorporated elements similar to Recurrent Neural Networks (RNNs). Additionally, I employed feature engineering techniques to extract new features from the data to enhance the model's performance.

One crucial aspect of the algorithm was object tracking, where the focus was on tracking the coordinates of each player's helmet. By analyzing the movement patterns, the model could identify specific motion characteristics indicative of player contact. For instance, rapid decreases in relative velocity after contact or significant changes in direction or orientation were considered as potential signs of contact.

## Expanding to Video Data

While my submitted code successfully handled tracking data, my future plans involve expanding the approach to incorporate video data using the YOLOv5 algorithm. This enhancement will enable more comprehensive and accurate detection of contact incidents in the National Football League of America, with the ultimate aim of minimizing harm and injuries.

## Competition Submission

The competition required participants to submit a valid sample submission file in CSV format. The submission file included a "contact_id" column, which combined the game_key, play_id, nfl_player_ids, and step (as explained earlier). The "contact" column contained binary values, with 1 indicating contact detected and 0 indicating no contact.
