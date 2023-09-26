# MQTT Guide

For communication using MQTT, follow the steps below:

1. Install Mosquitto from the link https://mosquitto.org/download/.

2. Start the server by typing ``` Mosquitto``` in the terminal/cmd.

3. For publishing messages to a topic, expand the libraries list and click on the Communication library.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt1.png?raw=true" align="middle" width="800" height="400"></a>

4. Drag and drop an MQTT Publish node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt2.png?raw=true" align="middle" width="800" height="400"></a>

5. From the Basic library, drag and drop a Start node and an End node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt3.png?raw=true" align="middle" width="800" height="400"></a>

6. On the MQTT Publish node, set the broker to localhost, port to 1883, topic to simpleflow/mqtttest, and message to "hello world".

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt4.png?raw=true" align="middle" width="800" height="400"></a>

7. Subscribe to the same topic to check if the message is sent. [Node-RED](https://nodered.org/) was used here to subscribe to the topic.

8. Execute the flow.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt5.png?raw=true" align="middle" width="800" height="400"></a>

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt6.png?raw=true" align="middle" width="800" height="400"></a>

9. For subscribing to a topic and receiving messages, expand the libraries list and click on the Communication library.

10. Drag and drop an MQTT Subscribe node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt7.png?raw=true" align="middle" width="800" height="400"></a>

11. On the MQTT Subscribe node, set the broker to localhost, port to 1883, and topic to simpleflow/mqtttest.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt8.png?raw=true" align="middle" width="800" height="400"></a>

12. Publish to the same topic to check if the message is sent. [Node-RED](https://nodered.org/) was used here to publish to the topic.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt9.png?raw=true" align="middle" width="800" height="400"></a>

13. Execute the flow.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/mqtt10.png?raw=true" align="middle" width="800" height="400"></a>
