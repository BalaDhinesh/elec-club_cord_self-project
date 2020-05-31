# Problem Statement:
To make a simple device which alerts the user when he touches his face using his hands. This device helps us to prevent coronavirus spread.

# Team Members:

1. [DHINESH](https://github.com/BalaDhinesh)
2. [SHARANESH](https://github.com/rsharanesh-iitm)

## Description of the project:
On an average, people touch their face 23 times per hour using their hands. In the age of coronavirus, we all have to resist the urge to touch our faces because there is a very high risk of getting affected by coronavirus due to germs present in our hands. But it is diffcult for people to develop this habit since without our knowledge, we have the habit of touching the facial parts often. One way to avoid doing this habit is to develop another habit of not touching their face. So, we decided to come up with an idea to develop the training of not touching their face by a device.


This is a small disposable electronic device that attaches to a users wrists and will monitor hand motion and when the hand position is close to face (Above the shoulders) will emit a small, harmless electrical pulses (no more than 1 Second) to that wrist or Vibrational Stimulus.  This electrical pulse or small vibration is intended to silently alert user that their hands are in close proximity to the face.  It is designed for easy to use user experience to lightly remind users to refrain from unnecessarily touching their mouth, nose, and eyes.



Two devices are needed to have it on both hands. However, we can use a single device by wearing in the hands alternatively. The goal is to get to avoid the habit of touching the face.


## Components Required:
- Microchip ATtiny85
- Accelerometer LIS2DH12TR
- CR1220 3V Lithium Coin Cell
- Push button(one for power on and one for load)



## Ideation:
A low power accelerometer is used to continuously monitor the hands motion. Microcontroller is used to store the information and helps as to when to produce electrical pulses/vibrations. Basically the device will calibrate the face position(accelerometer value) when power button is pressed and keeping the device near the face. Now, it is calibrated and stored the value in the microcontroller. Some coding part has to be done in the microcontroller for some range of values near to the calibrated value(For more accurate measurements, we can calibrate different parts like nose, mouth, eyes etc.,). It is then ready to use.

When the power on button is pressed, the device is ready for calibration. To calibrate, keep near the face the device and push the load button. Now the device note the accelerometer readings. Now, the microcontroller sets some threshold values in all 3 axis. The device is now ready to use. whenever the user places his/her hand near their face, the device produce an electric pulse to alert the user. 

If the user wants to change the position, load button should be pressed again keeping the hands near to his hands to calibrate it again.



This prototype will work perfectly only when he is static or moving with the same height from the basement. However in most cases in our daily routine like studying, at classroom, playing sports etc., the height from the basement will be almost be the same. If we want change our position(like changing the position from sit to stand or vice-versa), it is very simple to calibrate it again by just pressing the button.






## Design:
This prototype should be able to wear in the user's hands for a longer period of time. So, the material outside the prototype should be in such a way that it doesn't irritate the person's skin. For this, we use silicone to cover the top layer. 

__Here is an idea of approach on how the product finally look like:__

![](https://hackster.imgix.net/uploads/attachments/1102401/ks5094416709_110_kHyoq33Eic.jpg?auto=compress%2Cformat&w=740&h=555&fit=max)


![](https://hackster.imgix.net/uploads/attachments/1102402/ks969411919_106_copy_NQhzvwtCQE.jpg?auto=compress%2Cformat&w=740&h=555&fit=max)


## Feasibilty check:
- From the document of ATtiny85, it is shown that this microcontroller can be operated between 2.7-5.5 volts. Hence power supply by two 3V coin cell battery is more than enough to operate.


## Datasheets:
1.[ATtiny85](http://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-2586-AVR-8-bit-Microcontroller-ATtiny25-ATtiny45-ATtiny85_Datasheet.pdf)

2.[LIS2DH12TR](https://www.st.com/en/mems-and-sensors/lis2dh12.html)


## Ideas inspired from the following links:

1.https://www.hackster.io/shockbit1/shockbit-1f46e4

2.https://immutouch.com/
