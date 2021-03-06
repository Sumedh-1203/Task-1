# Project-1: [Facial Recognition Door Using Windows IOT](https://www.hackster.io/windows-iot/windows-iot-facial-recognition-door-e087ce)

**Problem Statement:** Designing a device that unlocks itself if it recognizes the face in front of the door camera and stays locked if it doesnt recognize the face.

**Ideation and Planning:** Understanding the working of the device
- *Doorbell -> Webcam -> PC -> Facial recognition API -> Microcotroller -> Relay switch -> Door*

**Part of the pipeline to break**

| Part of the Pipeline   | Feasibility                                                                                                        | Advantages                                                                                                                                        | Disadvantages                                                                                                  |
|------------------------|--------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Camera                 | Webcams are moderately expensive and very easy to set up.                                                          | Webcams will provide very high quality images making the facial recognition very accurate.                                                        | Webcams can be hacked quite easily which gives rise to security issues.                                        |
| PC                     | For this project any PC with an internet connection and windows 10 will do.                                        | A PC will make setting up the code very easy and faces which are to be recognized by the camera can be registered without much hassle.            | It can be very expensive to buy a new PC in case someone doesnt have one from before.                          |
| Facial recognition API | Face detection will become very easy using an API.                                                                 | Very easy to implement. Even people who have no idea about machine learning can use it.                                                           | There is the risk of the data getting leaked and thus breaching the privacy of people visiting your house.     |
| Microcontroller        | In this project, the Raspberry Pi is used. It is a low cost development board which is easily available in market. | The Raspberry Pi supports many interfaces like WiFi, USB, GPIO, bluetooth etc and also supports python making it very easy to build applications. | Raspberry Pi needs a bit of prior knowledge about linux and python and is not very easy to code for beginners. |
| Relay switch           | Relay switches are very cheap and the motion of the door can be controlled very easily using a relay switch.       | Very easy to install and low power consupmtion.                                                                                                   | It can get damaged if high current is inputted.                                                                |

**Choosing a pipeline:** 
From the above we can choose the Camera for improvements. 

*Webcam-* 
- If a normal webcam is used, the door will unlock even if we show the camera a photo of a person instead of the actual face. 
- To overcome this issue, we can either use a depth camera or add a finger print reader for extra security.


# Project-2: [Density Based Traffic Signal System Using Microcontroller](https://www.electronicshub.org/density-based-traffic-signal-system-using-microcontroller/)

**Problem Statement:** Designing a device that measures traffic density on the road and operates the signal accordingly to reduce traffic congestion at an intersection.

**Ideation and Planning:** Understanding the working of the device
- *IR sensor -> Microcontroller -> Traffic light*

**Part of the pipelone to break:**

| Part of the Pipeline    | Feasibility                                    | Advantages                                            | Disadvantages                                            |
|-------------------------|------------------------------------------------|-------------------------------------------------------|----------------------------------------------------------|
| IR Sensor               | Cheap and easily available in the market.      | Very easy to set up and low power consumption.        | IR sensors can detect objects at a short range.          |
| ATmega8 Microcontroller | This microcontroller is cheap and easy to use. | Many tutorials and proper documentation is available. | Has less computational capabilities compared to arduino. |
| Traffic light           | Easily available and cheap.                    | Will help in reduce congestion on road.               | Can get damaged due to external factors like rain etc.   |

**Choosing a pipeline:** 
From the above we can choose the IR sensor for improvement.

*IR Sensor-*
- IR sensors have a short range so cannot detect traffic at very long ranges.
- Instead of IR sensor we can have a camera which can measure the traffic density using computer vision and time the signals accordingly.