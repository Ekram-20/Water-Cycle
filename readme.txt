------------------------------------------------------------
about the project:
title: Water Cycle (Computer Graphics Project)
PlatForm: Visual Studio
Operating System: Windows


brief:
it's a demonstration of the water cycle and different types of precipitation, rain, sleet and snow
project will start playing as soon as you run it and will keep looping until the window is closed.
------------------------------------------------------------

------------------------------------------------------------
functions:
void display():
calls all the drowing functions and create the scenes
-------------------------
//for the background scene
void ground():
a 3d cuboid wraped in a ground texture on the sides, grass on top and dirt on the bottom
-------------------------
void lake(radius, num_vertex):
takes the radius to draw a 2d circle for the lake
-------------------------
void mountain():
3d mountains using multiple pyramids, covered in a texture.
-------------------------
void oneCloud():
3d spheres in different sizes shaping a cloud
-------------------------
void clouds():
multiple clouds in multiple positions using oneCloud()
-------------------------
void rocks():
3d Dodecahedron rocks set by the lake, colored in black
-------------------------
void sun():
3d sphere using quadratic, covered with sun texture eand surronded by an aura
-------------------------
void tree():
3d tree drawn using 3 cones and a cylinder for the trunck, upper tree cone go white when it's snowing
-------------------------
void waterfall():
2d waterfall using quads, wraped in waterfall texture, flowing under the mountains
-------------------------

//evaporating
void arc():
draws an arc using line strip, used as a base for the steam
-------------------------
void steam():
drawing mutiple arcs to visualize steam
-------------------------
void evaporate():
make the vapor arcs go up for the evaporating part and disappear down when it's done, at the beginning when variable t < keyFrameTimes[1]
-------------------------

//condensing
void condense():
make the weather cloudy, by changing the background color to a darker blue shade and moving the clouds closer and grayer in color
-------------------------

//raining
void drop():
a 3d rain drop, drawn using a cone and a sphere
-------------------------
void rain():
start a scene of rain (multiple raing drops, under the colud) after the steam and cloud condesing when variable t between keyFrameTimes[2] and keyFrameTimes[3]
-------------------------
void raining():
start raining by calling the precipiting function and passing the raining speed to it
-------------------------

//sleeting
void sleet():
drawing the sleet scene with multiple sleets using spheres after the raining part when variable t is between keyFrameTimes[3] and keyFrameTimes[4]
-------------------------
void sleeting():
start sleeting by calling the precipiting function and passing the sleeting speed to it
-------------------------

//snowing
void iceCrystal():
drawing a snowflake using multiple lines
-------------------------
void snow():
drawing the snow scene with multiple snowflakes after the sleeting part when variable t is between keyFrameTimes[4] and keyFrameTimes[5]
-------------------------
void snowing():
change the background color and start snowing by calling the precipiting function and passing the snowing speed it,snow then moves down making the ground go white as snow fills it
-------------------------
void montainSnow():
drawing a white cone on the summet of the mountain when it snows.
-------------------------

//miscellaneous
void precipiting(speed):
Adjust the speed for each type of precipitation, based on the speed passed to the function
----------------------------------
void quadTexture(v1[],v2[],v3[],v4[],texture):
takes 4 3d points and a texture to draw a quad shape covered in texture, used to draw the waterfall
--------------------------
void drawPyramid():
draws a 3d pyramid used to draw the mountains
-------------------------
void key(key, x, y):
press x,X to decrease/increase camera x position
press y,Y to decrease/increase camera y position
press z,Z to decrease/increase camera z position
--------------------------
void translate(x, y, z, shapeFunction):
takes the translation values x,y,z and the drawing function to translate the shape based on the specified amount
--------------------------
void scaleAndTranslate(tx, ty, tz, s, shapeFunction):
takes the translation values tx,ty,tz , the scaling value s and the drawing function to preform uniform scaling and translate the shape based on the specified amounts.
---------------------------------------------------------

