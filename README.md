# Video Frame Classification Using Deep Learning


## Model Information
The model used for classification is saved as "ufc_classifier_model.h5". It was initially planned to use ConvLSTM for better sequential video analysis, but due to limited GPU power, Conv2D was used instead. The model works with single frames extracted from videos to classify them into different sports and activities
initially model takes an image or an input , using 4lakh parameters model achieve the accuracy of 95 percent without any overfitting with less gpu cost.

dur to less gpu it is not possible to process video frame by frame so an idea to take 15 frame (formally 5 but dataset become large and need more comptuational cost) make it even to achieve the accuracy and poredict the classes accuractely on new testing data(taken randomly from google)

## How to Use
1. Input a video file.
2. The script extracts a frame from the video.
3. The frame is resized and preprocessed.
4. The model predicts the activity.
5. The predicted activity label is displayed.

## Activity Classes
```
BaseballPitch, Basketball, BenchPress, Biking, Billiards, BreastStroke, CleanAndJerk, Diving,
Drumming, Fencing, GolfSwing, HighJump, HorseRace, HorseRiding, HulaHoop, JavelinThrow,
JugglingBalls, JumpRope, JumpingJack, Kayaking, Lunges, MilitaryParade, Mixing, Nunchucks,
PizzaTossing, PlayingGuitar, PlayingPiano, PlayingTabla, PlayingViolin, PoleVault, PommelHorse,
PullUps, Punch, PushUps, RockClimbingIndoor, RopeClimbing, Rowing, SalsaSpin, SkateBoarding,
Skiing, Skijet, SoccerJuggling, Swing, TaiChi, TennisSwing, ThrowDiscus, TrampolineJumping,
UCF50, VolleyballSpiking, WalkingWithDog, YoYo
```

## Notes
- The extracted frame must match the model’s required input size.
- Modify frame extraction settings if necessary.
- Ensure correct label mapping for accurate predictions.

## License
This project is open-source and intended for educational use.


