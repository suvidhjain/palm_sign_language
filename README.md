# palm_sign_language
Palm Sign Language project based on Machine Learning CNN. 

1. Start the project by making virtual enviorment from pip and then open the app in that location or directory.
Note: use python version 3.6 and 64bit 

2. Then install requirements.txt file through pip in virtual env.
                pip install -r requirements_cpu.txt
Note: always use a virtual env for not getting dependency errors it will waste your time.

3. Data for the alphabets have been already made in it you can add more through create_gestures.py.

4. Run python set_hand_hist.py file before running the main file that is recognize_gesture.py this file is basically used whenever the lighting condition or hand changes.
Basicaly the work of set hand histogram is to convert the whole coloured image into the grayscale image.
  
  A windows "Set hand histogram" will appear.
  * "Set hand histogram" will have 50 squares (5x10).
  * Put your hand in those squares. Make sure your hand covers all the squares.
  * Press 'c'. 1 other window will appear "Thresh".
  * On pressing 'c' only white patches corresponding to the parts of the image which has your skin color should appear on the "Thresh" window. 
  * Make sure all the squares are covered by your hand.
  * In case you are not successful then move your hand a little bit and press 'c' again. Repeat this until you get a good histogram.
  * After you get a good histogram press 's' to save the histogram. All the windows close.
  
5. Train your model through:

  python cnn_tf.py
  or
  python cnn_keras.py
 
But, we wern't be able to implement train our model via  
Tensorflow.
Note: you have to retrain your model everytime whenever you add or delete any gesture.
