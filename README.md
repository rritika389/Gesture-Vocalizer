# Gesture Vocalizer 
* The flex sensor measures the bending of fingers according to gesture and outputs change in resistances corresponding to the amount of bending.
* Accelerometer sensor measures the linear movements of hand in X-axis and outputs different values of X corresponding to the movement in X-axis. 
* Touch sensor measures if there is any contact between two fingers.
* All the data from sensors are then processed on Arduino UNO involves combination of all the sensor outputs in order to match the resultantoutput with pre-stored values of different signs regarding the alphabets. 
* For this, appropriate ranges are set for each alphabet and the words that can be recognized with single hand based on the measured data obtained from repeated measurements.
* A Bluetooth module is connected to Arduino UNO. The Processed data are then transferred to the Bluetooth module (transmitter) obtained in string format. 
* The Android mobile also have an inbuilt Bluetooth capability. 
* These two Bluetooth devices are then paired, and string is transmitted to Android mobile.
* Android mobilereceives data via Bluetooth in bytes format, convert them into string.
* Finally, the string is converted into voice using the text to speech application of Android mobile.
* This overall system is mounted over a normal glove for easy handling and recognizes
the hand gestures accurately.
* The overall process can be summarized as follows:
1. The user performs hand gestures while wearing the sensor-equipped gloves or
device.
2. The flex sensors capture the hand movements and generate electrical signals.
3. The Arduino Uno microcontroller receives the sensor signals and processes them
using the gesture recognition algorithm [7].
4. The identified gesture is sent to a mobile application using a Bluetooth module
which converts it into corresponding text.
5. The mobile application also generates synthesized speech, which is output through
the speaker.
