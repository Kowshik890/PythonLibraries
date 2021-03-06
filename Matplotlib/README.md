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
  * **plt.subplot(subplot(nrows, ncols, index)**
    * Example: 
         plt.subplot(211) or plt.subplot(2,1,1)
    * Here, 
          
           nrows = rows (maintain a distance between subplot and main plot and describe as number of plots also)
    
           ncols = divide the main plot into number(ncols)
           
               Example: if ncols = 1, that means the main plot is equal to subplot. 
               
                        if ncols = 2, that means the main plot is divided by 2. The subplot size will be half of the main plot.
                        
           index = the position of the subplot according to the main plot.
           
               Example: if ncols = 3 and index = 2, that means, the main plot will be divided by 3 and the subplot will be in the 2nd or middle position.
               
    * N.B: If we give the same value of two subplot function, one will be overwrite by the existing one.
 * **fig.add_subplot(nrows, ncols, index, facecolor='color name')**
   * Example: 
        fig.add_subplot(221, facecolor='y')   # Here, facecolor = 'y' (yellow) is used for the background color for the subplot.
   * The add_subplot() function of the figure class will not overwrite the existing plot.
 * N.B: You can add an insert plot in the same figure by adding another axes object in the same figure canvas.
  
 **5. [Subplot2grid() Function](https://www.tutorialspoint.com/matplotlib/matplotlib_subplot2grid_function.htm)**
  * **plt.subplot2grid(shape, location, rowspan, colspan)**
    * Subplot2grid() Function is used to span across multiple rows or columns.
  * **plt.tight_layout()**
    * Used to maintain a proper distance from one plot to another
 
 **6. [Grids](https://www.tutorialspoint.com/matplotlib/matplotlib_grids.htm)**
  * figsize(width, height) --> figure size
  * lw = linewide (Width or density of the curved line)
  * ls = linestyle (for example: '.', '--', '-.' etc)
  * grid(True) = default grid
  * for customize of grid() [color, ls(linestyle), lw are the parameters]
  
 **7. [Formatting Axes](https://www.tutorialspoint.com/matplotlib/matplotlib_formatting_axes.htm)**
  * **axes[1].set_yscale("log")**
    * this syntax will help to set the large curve in y axis
  * **axes[0].xaxis.labelpad = 10**
    * Distance between axis numbers and axis label is 10 in X axis from axes[0]
  * **Axis spines**
    * The axes object has spines located at top, bottom, left and right.
    * Each spine can be formatted by specifying color and width.
    * Any edge can be made invisible if its color is set to 'None'.
      * for example: ax.spines['right'].set_color(None)    # This edge will be invisible
  
 **8. [Twin Axes](https://www.tutorialspoint.com/matplotlib/matplotlib_twin_axes.htm)**
  * **a2 = a1.twinx()**
    * the value of X axis will be remain same for both curves
    * in "twiny()" function, the value of Y axis will be remain same for both curves
 
 **9. [Bar Plot](https://www.tutorialspoint.com/matplotlib/matplotlib_bar_plot.htm)**
  * **ax.bar(x, height, width, bottom, align)**
    * x      = input value
    * height = output value (y axis)
    * width  = bar size in wide
    * bottom = from where it will start
    * align  = {'center', 'edge'}, optional, default 'center'
  * pyplot.bar() function allows to specify a starting value for a bar
 
 **10. [Histogram](https://www.tutorialspoint.com/matplotlib/matplotlib_histogram.htm)**
  * **ax.hist(a, bins = [0,25,50,75,100])**  
    * Bin the range of values
  * To construct a histogram, follow these steps −
    * Bin the range of values.
    * Divide the entire range of values into a series of intervals.
    * Count how many values fall into each interval.

 **11. [Pie Chart](https://www.tutorialspoint.com/matplotlib/matplotlib_pie_chart.htm)**
  * **pie(x, labels, colors, autopct)**
    * x       = array-like. The wedge sizes.
    * labels  = list. A sequence of strings providing the labels for each wedge.
    * autopct = the format for numbers %1.2f% 
    * For example: ax.pie(students, labels = langs,autopct='%1.2f%%') # color is optional parameter

 **12. [Scatter Plot](https://www.tutorialspoint.com/matplotlib/matplotlib_scatter_plot.htm)**
  * **scatter(data range, data, color)**
    * For example: ax.scatter(grade_range, girls_grades, color = 'b')
