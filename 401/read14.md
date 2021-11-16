# Matplotlib
package for 2D-graphics to draw plots

You can control the defaults of almost every property in matplotlib: figure size and dpi, line width, color and style, axes, axis and grid properties, text and font properties and so on.

**some of plt properites**

- color property to change line color
- linewidth property to change line thikness

**some of plot commands**

- `plt.xlim(X.min()*1.1, X.max()*1.1)` to set limits for x-axis
- `plt.xlim(X.min()*1.1, X.max()*1.1)` to change how gradients look like
- `ax.spines['bottom'].set_position(('data',0))` to change the position of cartesian
- `plt.legend(loc='upper left', frameon=False)` to add a key for explaining
- `plt.annotate()` to declare some points on the graph

## figures


|Argument      |  Default               |  Description                                 |
|--------------|------------------------|----------------------------------------------|
|num           |   1                    |   number of figure                           |
|figsize       |   figure.figsize       |   figure size in in inches (width, height)   |
|dpi           |   figure.dpi           |   resolution in dots per inch                |
|facecolor     |   figure.facecolor     |   color of the drawing background            |
|edgecolor     |  figure.edgecolor      |  color of edge around the drawing background |
|frameon       |   True                 |   draw figure frame or not                   |


## Subplots
With subplot you can arrange plots in a regular grid.

## Axes
allow placement of plots at any location in the figure



---------------------------------


# Bokeh
Bokeh is an interactive visualization library that targets modern web browsers for presentation