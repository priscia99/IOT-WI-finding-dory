# IoT/WI - Finding Dory - Final Project [A.Y. 2021/2022]
This is the final project regarding the courses **Internet of Things** and **Wireless Internet**, A.Y. 2021/2022.
## 💡 Introduction
The main purpose of the project is to find the coordinates $(X, Y)$ of the position of *Dory* by using a **fingerprint dataset** composed of Received Signal Strength Indicator (**RSSI**) values from six *sniffer-anchors* and the RSSIs emitted by Dory’s smartphone in its corresponding coordinates.

The fingerprint dataset has been divided into small fragments of data hidden inside **MQTT publishes/subscriptions** and **CoAP request/response** packets and it was required to obtain all these fragments, clean them and remove the outliers.

After reconstructing the entire fingerprint dataset, it was necessary to find a model that was able to determine the position of the device with the most similar fingerprint, comparing the RSSI measurements from Dory’s device with the database’s entries.

This model, implemented within a **Python** script, exploits the **Euclidean Distance** to find the final coordinates $(X,Y)$ of Dory.
