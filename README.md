# Saving Lives using Computer Vision and the CAN BUS

This project details a possible solution for a serious problem around the world that can potentially resolve or at least reduce the number of deaths due to Pediatric Vehicular Heatstroke (PVH). The proposed system uses a microcontroller-based platform, computer vision, wireless communication notification, and the integrated second-generation on-board diagnostic port (OBD-II), totaling a cost less than \$450.00 U.S. dollars.

To limit the scope, the initial phase of the project is to create a system to perform real-time object detection limited to identifying pets (dogs and cats) left unattended in a vehicle setting. Upon positive detection of an unattended pet in the vehicle, the system transmits an email and short message service (SMS) via Wi-Fi to the pet owner's cellular phone and email address. Also, based on the current interior temperature, corrective action is taken via the vehicle's climate control system. In the current implementation, the system can successfully adjust the vehicle's ambient temperature if its measured to be above the appropriate temperature threshold for the pet. The system's main platform, Raspberry Pi 4B, is utilized since it was the less expensive, yet powerful microcontroller running on programming language, python. Also, provided most of the features needed throughout the project such as USB 3.0, Micro SD Card Slot, integrated 2.4/5 GHz Wireless Module, a 2-lane Camera Serial Interface (CSI) camera port, 40 Pin general-purpose input/output (GPIO) header, and USB-C Power Port (5V/3A). Resulting in easy integration of other components such as the Intel Movidius Neural Compute Stick II, DTH22 temperature and humidity sensor, camera, and wireless communication. For the computer vision portion of the system, the team concluded to use Tiny-YOLOv3 real-time object detection model due to the fact that the model can be deployed on an inexpensive microcontroller without a graphics card and limited memory. Lastly, in order to control the vehicle's climate control system, the approach of using a PiCAN module was chosen since it is a direct attachment to the GPIO header of the microcontroller.

In terms of improvements, the project could be expanded to detect children as well. Also, instead of using an average camera for object detection, a 360\degree camera can be considered since it can cover more area at once.

Project Developers:
Daniel Jacuinde-Alvarez (CSU, Fresno) and James Dols (CSU, Fresno)



Paper: https://drive.google.com/file/d/1DAk3_kKkFyRtHwXDpqd4jXwFziAJWpMC/view?usp=sharing 
