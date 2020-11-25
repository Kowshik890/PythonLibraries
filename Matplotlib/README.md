# Matplotlib Learning & Practicing

## Topic's Name 

**1. [PyLab Module](https://www.tutorialspoint.com/matplotlib/matplotlib_pylab_module.htm)**
  * **Basic Plotting**
    * Plotting curves is done with the plot command
  * **Multiple Plotting Curves**
    * Plots can be overlaid. Just use the multiple plot commands.
  
**2. [Object-oriented Interface](https://www.tutorialspoint.com/matplotlib/matplotlib_object_oriented_interface.htm)**
  * **fig = plt.figure()**
    * create a figure instance which provides an empty canvas.
  * **ax=fig.add_axes([0,0,1,1])**
    * The add_axes() method requires a list object of 4 elements corresponding to left, bottom, width and height of the figure. 
    * Each number must be between 0 and 1
  
**3. [Axes Class](https://www.tutorialspoint.com/matplotlib/matplotlib_axes_class.htm)**
  * **ax.legend(handles, labels, loc)**
    * Example: ax.legend(labels = ('tv', 'Smartphone'), loc = 'lower right')
    * Location: (String - Code)
      * Best - 0, upper right	- 1, upper left	- 2, lower left	- 3, lower right - 4, Right	- 5, Center left	- 6, Center right	- 7, lower center	- 8, upper center -	9, Center -	10
  * **axes.plot()**
    * Example: ax.plot(x1,y,'ys-')
    * Color codes
      * ‘b’	- Blue, ‘g’	- Green, ‘r’ -	Red, ‘c’ -	Cyan, ‘m’ -	Magenta, ‘y’	- Yellow, ‘k’ -	Black, ‘w’ -	White
    * Marker codes
      * ‘.’	- Point marker, ‘o’ -	Circle marker, ‘x’ -	X marker, ‘D’ -	Diamond marker, ‘H’	- Hexagon marker, ‘s’ -	Square marker, ‘+’ -	Plus marker
    * Line styles
      * ‘-‘	- Solid line, ‘—‘ -	Dashed line, ‘-.’ -	Dash-dot line, ‘:’ -	Dotted line, ‘H’ -	Hexagon marker

 **4. [Multiplots](https://www.tutorialspoint.com/matplotlib/matplotlib_multiplots.htm)**
