# People Movement Prediction Framework


The ability to accurately predict people movement is crucial to numerous domains such as wireless networks, HCI, social science, urban planning, transportation, etc. While predicting the movement of a person, we seek the answers to three fundamental questions: (1) where will the person stay at a future time (i.e., location)?, (2) How long will she stay at the location (i.e., stay duration)?, and (3) Who will she meet (i.e., contact)? Providing answers to three questions altogether remains challenging due to the: (1) complex nature of people movement, and (2) lack of a realistic people movement trace used to construct an accurate predictive model of people movement. On the other hand, it is believed that people movement exhibits a high degree of repetition, in which people visit regular places for their daily activities. 

In this work, we deployed the a scanning system on Google Android phones to collect MAC addresses of Wifi access points and Bluetooth devices in the proximity of the experiment participants. We observe that Wifi access point information can be used to infer location while Bluetooth MACs can be used to infer contact. The joint Wifi/Bluetooth trace thus can be used to study people movement. 

The below figure shows steps of the framework to construct the predictive model of people movement from the joint Wifi/Bluetooth trace. In the first and the second steps, we cluster Wifi records in into locations. Then, in steps 3 and 4, we construct a Naive Bayesian classifier to assign locations for records in Bluetooth trace. In steps 5 and 6, the Bluetooth trace with assigned location is used as the input to construct a location predictive model, a stay duration predictive model, and a contact predictive model.



![testing](https://github.com/lhvu2/movement_prediction_framework/blob/main/images/movement_prediction_step.png)



# Reference

1. "Jyotish: A novel framework for constructing predictive model of people movement from joint wifi/bluetooth trace", Long Vu, Quang Do, Klara Nahrstedt, EEE International Conference on Pervasive Computing and Communications, 2011

2. "Joint bluetooth/wifi scanning framework for characterizing and leveraging people movement in university campus", Long Vu, Klara Nahrstedt, Samuel Retika, Indranil Gupta, ACM international conference on Modeling, analysis, and simulation of wireless and mobile systems, 2010

3. "Characterizing and modeling people movement from mobile phone sensing traces", Long Vu, Phuong Nguyen, Klara Nahrstedt, Björn Richerzhagen, Pervasive and Mobile Computing Journal, 2015

4. "Jyotish: Constructive approach for context predictions of people movement from joint Wifi/Bluetooth trace", Long Vu, Quang Do, Klara Nahrstedt, Pervasive and Mobile Computing Journal, 2011
