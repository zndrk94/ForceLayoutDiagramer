# ForceLayoutDiagramer

**This project is still a work in progress and porbably won't be useful to anyone yet, so if you need something to be usefull now, look elsewhere**

This is force layout diagram I made in C++ using OpenGL. It's works okay, but it could use some improvement. 
I'm actually in process of turning this into a more robust Python library and hope to have that done in a month at most. 

**How to run**

You need to use the following flags like so: 

`g++ -std=c++11 graph.cpp -lglut -lGL -lGLEW -lGLU -o graph`

Date is read in from `dataPoints.csv` which are currently random points (-1 < x < 1)

Running 2D and 3D varry slightly in terms of specifying the stepping rate of the simulation. 

For 2D: The stepping rate is specified in the source code (`line 186` in `graphPoints.h`)

  `shell> ./graph`

For 3D: The stepping rate is specified in `argv[1]` and I suggest using `0.0002`. 

  `shell> ./graph 0.0002`
  
Once the program is running (2D and 3D), you can move around with your mouse so long as you click and drag. Use the keys `W`, `S`, `A`, and `D` to move *forwards*, *backwards*, *left*, and *right*. To get the points to *run* and move to equalibrium, press `N`. You will need to move backwards at first since the camera position is placed in the center of the box. Once you move backwards some, you'll be able to see the points and stuff. 
  

This projected is licensed under the terms of the MIT license.