# Node-Red_QLab
Node-Red control of Qlab and Qlab returning to Node-Red 

There are two switches connected to the GPIs of the Rasperry Pi along with a DHT22.  The GPIs enter the flow and depending on if they are depressed for a long or a short time they behave in a momentary or latching behaviour.

These inputs are passed to figure53 Qlab where certain actions happen. Within these actions are commands that return to the Node-Red flow.

These returns from Qlab trigger the GPOs which are connected to the two LEDs

The Node-Red flow is also contains a Dashboard which shows the state of the switches allows for a visual conformaiton they are working and to operate the swithces from the UI.

THe Node-Red dashboard also displays the metrics of the pi and the DHT22 sensor.
