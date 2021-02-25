# Expert-Novice Soccer Dataset

The dataset for the following paper:
Y. Akamatsu, K. Maeda, T. Ogawa, and M. Haseyama, “Classification of Expert-novice Level Using Eye Tracking and Motion Data via Conditional Multimodal Variational Autoencoder,” IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), 2021 (accepted for publication).

## Nine actions in our experiment
![Image 1](Experiment.png)

## Players

The total number of samples is 288 (= eight players * nine actions * four times).

|       | # Expert level samples | # Novice level samples | # All samples  |
| :----: |:------:| :------:| :-----: |
|Player1| 1 | 35 | 36 |
|Player2| 1 | 35 | 36 |
|Player3| 24 | 12 | 36 |
|Player4| 0 | 36 | 36 |
|Player5| 36 | 0 | 36 |
|Player6| 36 | 0 | 36 |
|Player7| 35 | 1 | 36 |
|Player8| 36 | 0 | 36 |
|All players| 169 | 119 | 288 |

- Player1-4 : Novice players
- Player5-8 : Expert players (more than 10 years of soccer experience)


## Eye tracking data
- EyeTrackingData/Player`<player index>`/S`<sample index>`/`<feature>`_vec.csv
  -  `<player index>` : 1-8
  -  `<sample index>` : 01-04 (Penalty kick), 05-08 (Free kick), 09-12 (Direct shot), 13-16 (Shot from a cross), 17-20 (Volley), 21-24 (Dribble (long)), 25-28 (Dribble (short)), 29-32 (Dribble (straight)), 33-36 (Juggling)
  -  `<feature>` : Vectors of eye tracking data in the following table.


| `<feature>`| Name | Description | 
| :---- |:------| :------| 
|ac0, ac1, ac2 (X-Y-Z coordinate system)| Accelerometer data | The accelerometer data indicates the rotation of the glasses [m/s^2].|
|gd00, gd01, gd02 (X-Y-Z coordinate system)| Gaze direction (left eye) | The gaze direction is a unit vector with origo in the pupil center. |
|gd10, gd11, gd12 (X-Y-Z coordinate system)| Gaze direction (right eye) | The gaze direction is a unit vector with origo in the pupil center. |
|Player4| 0 | 
|Player5| 36 | 
|Player6| 36 |
|Player7| 35 | 
|Player8| 36 |
|All players| 169 |

## Motion data
