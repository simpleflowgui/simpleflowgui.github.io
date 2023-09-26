# Flow Guide

To create your first flow, follow the steps below:

1. Expand the libraries list by clicking on the triangle on the upper right corner of the main UI.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow1.png?raw=true" align="middle" width="800" height="400"></a>

2. Click on the "Basic" library to show the list of nodes that it includes.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow2.png?raw=true" align="middle" width="800" height="400"></a>

3. Add a Start node by dragging and dropping it from the list.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow3.png?raw=true" align="middle" width="800" height="400"></a>

4. Click on the "Computer Vision" library to show the list of nodes that it includes.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow4.png?raw=true" align="middle" width="800" height="400"></a>

5. Drag and drop a Predict YOLO node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow5.png?raw=true" align="middle" width="800" height="400"></a>

6. Click on the "Basic" library again.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow6.png?raw=true" align="middle" width="800" height="400"></a>

7. Drag and drop an Output Image node, and then an End node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow7.png?raw=true" align="middle" width="800" height="400"></a>

8. Connect the Start node to the Predict YOLO node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow8.png?raw=true" align="middle" width="800" height="400"></a>

9. Connect the Predict YOLO node to the Output Image node and the End node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow9.png?raw=true" align="middle" width="800" height="400"></a>

10. Select "pre-trained" for model, "Detection" for mode, "YOLOv8n" for select model, and any image to perform prediction on such as an image of a plane for the parameters of the Predict YOLO node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow10.png?raw=true" align="middle" width="800" height="400"></a>

11. To execute the flow, click on the "Execute" button.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow11.png?raw=true" align="middle" width="800" height="400"></a>

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow12.png?raw=true" align="middle" width="800" height="400"></a>

To save the flow, click on the "Save Flow" button.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow15.png?raw=true" align="middle" width="800" height="400"></a>

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow13.png?raw=true" align="middle" width="800" height="400"></a>

To load the flow again, click on the "Load Flow" button.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow14.png?raw=true" align="middle" width="800" height="400"></a>

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/flow16.png?raw=true" align="middle" width="800" height="400"></a>

