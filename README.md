# Contact-Detection
This is my second competition in kagle in which players contact is detected based on distance,accleration,orientation and other factors and even through video we have to detect contact.Multiple dataset is given we have to found out contact at each step, each player and ground at multiple game play at frequency of 10 hz as one step.I successfully submitted the code.Based on this multiple features output 1 or 0 can be given as contact detection or not.

I have created algorithm which consists a part similar to RNN and used feature engineering to extract new features from videos.

I performed object tracking on each player's helmet and tracking coordinates of each player.The model track certain movement that decides contact between players at a particular frame by depending on some previous frames data and some next frames data similar to RNN (eg.The algorithm can derive knowledge of contact between two players where relative velocity decreases rapidly  after contact and other such parameters as direction or orientation change etc).


This is for national football league of america for detecing contact for harm and injuries.I am established my code on tracking data but i will adding my code more on video data by using YOLOv5

sample_submission.csv A valid sample submission file.

contact_id: A combination of the game_key, play_id, nfl_player_ids and step (as explained above)
contact: A binary value predicting contact. 1 indicates contact and 0 indicates no-contact.

DATASETS LINK-https://www.kaggle.com/competitions/nfl-player-contact-detection/data
