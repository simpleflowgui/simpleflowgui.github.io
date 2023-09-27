# Custom Library Guide

To create a custom library, follow the steps below:

1. Click on the triangle on the upper right corner on the main UI to expand the libraries list.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom1.png?raw=true" align="middle" width="800" height="400"></a>

2. Click on the plus icon above the Libraries label.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom2.png?raw=true" align="middle" width="800" height="400"></a>

3. Enter the name of the library to be created in the specified area. Notice that an underscore is used to represent spaces.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom3.png?raw=true" align="middle" width="800" height="400"></a>

4. Enter the name of a node to be added under the new library. Notice that an underscore is used to represent spaces.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom4.png?raw=true" align="middle" width="800" height="400"></a>

5. The new node name will be added on the left area under, click on the node name.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom5.png?raw=true" align="middle" width="800" height="400"></a>

6. For the input type dropdown menu on the right, select text input.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom6.png?raw=true" align="middle" width="800" height="400"></a>

7. Enter a name of the variable.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom7.png?raw=true" align="middle" width="800" height="400"></a>

8. Change the color of the node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom8.png?raw=true" align="middle" width="800" height="400"></a>

9. Click on Add. Notice that the name of the variable will be added on the left. Clicking on it will remove it.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom9.png?raw=true" align="middle" width="800" height="400"></a>

10. Click on Back.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom10.png?raw=true" align="middle" width="800" height="400"></a>

11. The following code lines will be used as an exampe to print a string in the log box. It should be noted that to access any of the variables defined when the custom node is created, the name of the variable will be used as a key for the vars dictionary as follows ```inps["vars"]["NameOfVariable"]```. Also, end the function code with a return statement to send the results back for further processing. To display an image, save the image data and assign the value to the key "data" in the returned object.

```
def Print_String(inps):
  writelog(inps["vars"]["String"])
  return{"string":inps["vars"]["String"]}
```

12. Paste the node function on the right.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom11.png?raw=true" align="middle" width="800" height="400"></a>

13. Click on create.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom12.png?raw=true" align="middle" width="800" height="400"></a>

14. Refresh the page, and the library will be added along with the node.

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom13.png?raw=true" align="middle" width="800" height="400"></a>

<a href="alternative text"><img src="https://github.com/simpleflowgui/simpleflowgui.github.io/blob/main/imgs/custom14.png?raw=true" align="middle" width="800" height="400"></a>

To add another node to the already created new library, follow the same steps but enter the name of the existing library.

Note: For all imports, classes, and global functions, paste the code in the text area under "Paste Imports" label

