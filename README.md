Download Link: https://assignmentchef.com/product/solved-cs224-assignment-4
<br>
For this assignment you will be creating a drawing program of your own. You are provided with a folder Artistik that contains the sample code. You will need to setup the project properties to use SDL2.0 to make this code work on your machines. How you can set up the project to use SDL2.0 can be learned by following the lazyfoo tutorials present at this <a href="http://lazyfoo.net/tutorials/SDL/">link.</a> Once everything is working, you will be able to draw a red rectangle by left clicking the mouse and dragging. The code is however incomplete as every time you draw a rectangle, the old rectangle is lost.:

In order to fix this issue, you will need to store every rectangle in a stack. As you keep on populating the stack, the number of rectangles will increase on screen. You are also given two structures for Point and Color as well. The tasks you need to accomplish are:

<ul>

 <li>You will need to declare a <strong>Shape </strong>base class</li>

 <li>Two classes <strong>Rect </strong>and <strong>Line </strong>will inherit from the Shape class. You will need to study SDL’s documentation to understand how a line is drawn. • You will create a <strong>Stack </strong>of your own</li>

 <li>Each node of the stack will only be able to store a pointer of type <strong>Shape</strong>. What this means is that whenever you will create a child object (either Rect or Line) its address will be passed to this base class’s pointer. As a result, the stack will be able to hold both Rect and Line objects.</li>

 <li>Every time you will create a line or a rectangle, it will have a random color (use the <strong>Color </strong>object for this reason).</li>

 <li>You will select what to draw by pressing ’r’ for Rect and ’l’ for line.</li>

 <li>You will undo with right mouse button whatever you draw by popping the stack.</li>

 <li>Whatever shape you pop, will be stored in a separate ”undo” stack</li>

 <li>You will redo with the middle mouse button which will pop the value from the ”undo” stack and push it in the first stack.</li>

 <li>if you undo and then draw some new shape, it will be added to the stack and subsequently purge the ”undo” stack.</li>

 <li>’-’ and ’+’ keys will change the order of the last drawn object within the stack. If you press ’-’ the shape will go deeper in the stack. If you press ’+’, the shape will start moving to the opt of the stack.</li>

</ul>

– The End –