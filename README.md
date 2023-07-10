# Contact-Detection
In my second Kaggle competition, the task was to detect player contact based on various factors such as distance, acceleration, orientation, and more. We were provided with multiple datasets, and the goal was to determine whether contact occurred or not at each step of the game, for each player and the ground. The data was collected at a frequency of 10 Hz.

To tackle this problem, I developed an algorithm that incorporated elements similar to Recurrent Neural Networks (RNNs). I also utilized feature engineering techniques to extract new features from the data.

One aspect of my algorithm involved object tracking, specifically focusing on tracking the coordinates of each player's helmet. By analyzing the movement patterns, the model could identify specific motion characteristics indicative of contact between players. For example, a rapid decrease in relative velocity after contact or significant changes in direction or orientation were considered as potential signs of contact.

The code I submitted successfully handled the tracking data, but my future plans involve expanding it to incorporate video data using the YOLOv5 algorithm. This will allow for more comprehensive and accurate detection of contact incidents in the National Football League of America, with the ultimate aim of minimizing harm and injuries.

The competition required participants to submit a valid sample submission file in CSV format. The submission file included a "contact_id" column, which combined the game_key, play_id, nfl_player_ids, and step (as explained earlier). The "contact" column contained binary values, with 1 indicating contact detected and 0 indicating no contact.

Overall, my approach involved leveraging RNN-like techniques, feature engineering, and object tracking to accurately predict player contact in the given datasets.
