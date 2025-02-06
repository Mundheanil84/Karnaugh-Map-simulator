# Karnaugh-Map-simulator
Abstract— 

This research paper proposes the design and 
development of a simulator to simplify Boolean expressions 
using Karnaugh Map (K-map). The simulator is developed 
using Html, CSS and JavaScript allows users to input Boolean 
expressions, display Karnaugh Map and output simplified 
Boolean expressions. The simulator is tested thoroughly and 
found to be accurate and efficient in simplifying Boolean 
expressions. The proposed simulator provides an effective tool 
for engineers and designers to simplify Boolean expressions, 
ultimately reducing the complexity of digital logic circuits.
Keyword – Boolean Expression, Karnaugh Map, Digital Logic 
Circuits,Virtual Simulator.

INNOVATIVE CONTENT

K-map, have been widely used in digital circuit design for 
decades. In this paper, Karnaugh map introduced a method for 
simplifying Boolean expressions using a two-dimensional 
map. The innovative content of Karnaugh's paper lies in the 
simplicity and effectiveness of the K-map technique, which 
allowed engineers to simplify complex digital circuits more 
efficiently than previous methods. Karnaugh's paper remains 
a cornerstone of digital circuit design, and K-map continue to 
be used today.

DEVELOPMENT OF SIMULATER

In this Experiment, simulator is developed by using HTML 
and JavaScript for K-map simplification tool. To develop this 
experiment, the first step would be to create an HTML file and 
add the necessary HTML elements such as buttons, input 
fields, and display areas as shown in Fig 2. CSS can be used 
to style the elements and create a visually appealing interface. 
The JavaScript code would then be added to implement the Kmap simplification algorithm. The code uses event listeners to 
detect user input and update the K-map and expression display 
accordingly [3]. The solveKMap() function is called when the 
user clicks the "Solve K-Map" button and it applies the QuineMcCluskey algorithm to the minterms and don't cares entered 
by the user [3] as shown in Fig 2 . The resulting prime 
implicants are displayed in the "notebook" textarea and the 
optimized expression is displayed in the "booleanfunction" 
div.

![image](https://github.com/user-attachments/assets/53cdd0cd-c1dc-4c1a-9b25-21775ab9b35d)

Fig 2. Selection of no. of variables
To develop this experiment simulation, the Second step would 
be to define variables to store the K-map data, such as the truth 
table and sequence of variables. The truth Table variable is an 
array that will hold all possible input combinations and their 
corresponding outputs. The sequence variable is an array that 
will hold the order of the variables in the K-map. The 
varCount variable is the number of variables in the K-map, 
which is set to 2 in this example [4] form Table 1 . The 
variables variable is a string that contains the letters A through 
H, which are used to label the variables. The k-Map variable 
is an array that will hold the visual representation of the Kmap, while cell Size, row, col, offsetX, and offsetY are 
variables used to determine the size and position of each cell 
in the K-map [4].

![image](https://github.com/user-attachments/assets/65862646-c017-4de1-99d5-3d3781b868d5)

Fig 3. Creation of truth table.
The function first calculates the coordinates of the clicked 
cell based on the mouse position and the size of the cells. It 
then checks if the cell is a valid one based on the number of 
rows and columns in the K-map [5] as shown in Fig 3. If the 
clicked cell is valid, the function converts the binary 
coordinates of the cell to a decimal index, and finds the 
corresponding input element in the HTML page [5]. It then 
toggles the value of the input element between 0, 1, and 'x' 
(don't care). After updating the input element, the function 
calls two other functions: writeMinterms() and createKMap()
[5]. WriteMinterms() updates the minterm and don't care lists 
based on the current input values, while createKMap() updates 
the visual representation of the K-map based on the input 
values as shown in Fig 3.
This function simplifyBooleanFunction() takes a Boolean 
function as input and returns the simplified version of the 
same Boolean function. It performs a series of simplification 
steps using Boolean algebraic laws and identities [5].
The input function is first checked if it is a constant (either 0 
or 1), in which case it is returned as it is from Table 1. 
Otherwise, it is stripped of any white spaces and all variables 
are converted to lowercase letters as shown Fig 1.
Fig 4. Simulator displays K-Map structure
The code assumes that the input values are already available 
in a truth table. It also assumes that the dimensions of the 
Karnaugh Map have been specified in row and col variables. 
The code uses the cellSize variable to specify the size of each 
cell in the HTML table that displays the Karnaugh Map [5] as 
shown in Fig 4. The variables and sequence variables are used 
to generate the Boolean expression. The output variable in 
create Boolean Function is used to store the final expression. 
The visited and K-map variables are used to keep track of 
which cells in the Karnaugh Map have been visited and their 
values.

![image](https://github.com/user-attachments/assets/3038677d-a365-4b5f-b5cf-acf4b773b2dd)


Fig 5. Simulator shows cells with values.
The function takes an optional parameter bg, which 
defaults to true. This parameter controls whether or not the 
background of the output values should be drawn. If bg is true, 
the function will draw a red square for each output value that 
is equal to 1, and a light red square for each output value that 
is a don't care ('x') [5]. If bg is false, the function will only 
draw the text of the output values. The function uses the push() 
and pop() functions to save and restore the current state of the 
canvas, so that any transformations applied to the canvas 
within the function do not affect other parts of the web page .
The function translates the origin of the canvas to the center 
of the Karnaugh map. The function then iterates over each cell 
in the Karnaugh map. For each cell, the function checks if the 
k-map array (which likely holds the current state of the 
Karnaugh map has a value at that cell. If it does, the function 
checks the value of that cell. If the value is 1, the function fills 
a red square at the center of the cell. If the value is 'x', the 
function fills a light red square at the centre of the cell. If bg 
is false, the function does not draw any squares as shown in
Fig 4 
