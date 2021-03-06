﻿# MLB-Pitch-Prediction
## Introduction

As an avid watcher of professional baseball, it is becoming more apparent that statistical data not only helps managers in making decisions, it has improved the consumption of the game. We can now get instantaneous visuals of where a pitch ends up, the trajectory of a ball going out of the park, and even probabilities of scoring based on the positions of runners and the number of outs. 

The goal of this project is to test the theory that pitches can be predicted based on the game situation. The implications of a successful outcome could lead to additional value to game consumption, or even a mobile application that would tell a user what pitch to predict based on the situation of the game (i.e.: runners on bases, inning, outs, pitch count, score, batter, pitcher, etc.). 

## Dataset

Kaggle is a great source of usable data in several subjects. The dataset used for this particular project is from a Kaggle dataset **MLB Pitch Data 2015-2018** at https://www.kaggle.com/pschale/mlb-pitch-data-20152018 . The dataset contains over 2.8 million observations over the three year period and includes .csv files such as _pitches_, _atbats_, _ejections_, _games_, _player_names_. 

For this specific project, we will utilize the _pitches_ and _at_bats_ datasets. The column descriptions for each dataset is below. Due to the size of the data and the limitations of processing the amount of data, the 2018 season will only be used as it would be the most relevant data as it is the most recent.

## Results

There are promising initial results and hope to continually improve. The image below is an example of a test sample result generated. The data in the top-left corner represents the game situation and the visual represents the pitch probability. Data points are:

- b_score = batter team score
- s_count = strike count
- outs = outs
- on_1b = runner on first base (1=True /0=False)
- on_2b = runner on second base (1=True /0=False)
- on_3b = runner on third base (1=True /0=False)
- batter_id = batter id number (matches to a batter name)
- inning = inning
- p_score = pitcher team score
- p_throws = pitcher stance (1=right /0=left)
- pitcher_id = pitcher number id (matches to a pitcher name)
- stand = batter stance (1=right /0=left)
- top = top of inning (1=True /0=False)
- b_count = ball count

![results example](https://github.com/Jason-Richards76/Baseball-Pitch-Prediction/blob/master/Untitled.png)

This file is too large for Github to fully support. You can access the notebook via Google Colaboratory at this address https://colab.research.google.com/drive/1VaHWXq2yYuH-S-6WL_WD8VFSugcgoiUz
