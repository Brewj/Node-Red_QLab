# Node-Red_QLab
Node-Red control of Qlab and Qlab returning to Node-Red 

The aim of this project was a remote location where there will be a local micriphone, this is connected via Dante back to our main audio DSP, the DSP is BSS SoundWeb and may be controlled directly but also may be controled from Qlab. As i don't have a soundweb unit on my desk Qlab is a good way of proving it's all working.

Components
-There are two switches connected to the GPIs of the Rasperry Pi along with a DHT22.  
-On the Raspberry Pi is Node-Red
-On my Mac i'm running Qlab.

The GPIs enter the flow and depending on if they are depressed for a long or a short time they behave in a momentary or latching behaviour.

These inputs are passed to figure53 Qlab where they open up the microphone to the appropiate zone. Within Qlab cues there are commands that return to the Node-Red flow. These returns from Qlab trigger the GPOs which are connected to the two LEDs to confirm to the operator that the microphone is live.

The Node-Red flow is also contains a Dashboard which shows the state of the switches allows for a visual conformaiton they are working and to operate the swithces from the UI.

The Node-Red dashboard also displays the metrics of the pi and the DHT22 sensor, as ultimatley this will be positiooned outdoors in a weather proof enclosure.

The Qlab files are included, along with a videos showing it in action.

## The Project
<img src="https://github.com/Brewj/Node-Red_QLab/blob/master/2020-04-03%2008.11.58.jpg" alt="picutre"></p>

## The Main Flow
<img src="https://github.com/Brewj/Node-Red_QLab/blob/master/Screenshot%202020-04-28%20at%2014.52.02.png" alt="main_flow"></p>

## The Stats Flow
<img src="https://github.com/Brewj/Node-Red_QLab/blob/master/Screenshot%202020-04-03%20at%2013.52.55.png" alt="stats_flow"></p>

## The Wiring Diagram
<img src="https://github.com/Brewj/Node-Red_QLab/blob/master/Wiring%20Diagram%20Fritzing_bb.png" alt="wiring_diagram"></p>
<img src="https://github.com/Brewj/Node-Red_QLab/blob/master/Wiring%20Diagram%20Fritzing_schem.png" alt="wiring_picture"></p>

## The Project in Action
https://youtu.be/xk8CGJNfmUY
