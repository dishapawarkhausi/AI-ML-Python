# Matplotlib Library - All Methods

This document provides a comprehensive list of methods available in Python's `matplotlib` library, categorized by their respective modules.

## 1. Matplotlib Pyplot Methods (`matplotlib.pyplot`)

```python
import matplotlib.pyplot as plt
```

- `plt.plot()` - Line plot
- `plt.scatter()` - Scatter plot
- `plt.bar()` - Bar chart (vertical)
- `plt.barh()` - Bar chart (horizontal)
- `plt.hist()` - Histogram
- `plt.boxplot()` - Box plot
- `plt.pie()` - Pie chart
- `plt.errorbar()` - Error bar plot
- `plt.fill()` - Fill area under curve
- `plt.fill_between()` - Fill between lines
- `plt.imshow()` - Display image data
- `plt.contour()` - Contour plot
- `plt.contourf()` - Filled contour plot
- `plt.clabel()` - Contour labels
- `plt.polar()` - Polar plot
- `plt.streamplot()` - Streamline plot
- `plt.step()` - Step plot
- `plt.stem()` - Stem plot
- `plt.hexbin()` - Hexagonal binning plot
- `plt.text()` - Add text to plot
- `plt.annotate()` - Annotate points
- `plt.xlabel()` - Set x-axis label
- `plt.ylabel()` - Set y-axis label
- `plt.title()` - Set title
- `plt.legend()` - Add legend
- `plt.colorbar()` - Add colorbar
- `plt.grid()` - Show grid
- `plt.xlim()` - Set x-axis limits
- `plt.ylim()` - Set y-axis limits
- `plt.xticks()` - Set x-axis tick labels
- `plt.yticks()` - Set y-axis tick labels
- `plt.subplots()` - Create figure with subplots
- `plt.subplot()` - Add subplot to figure
- `plt.figure()` - Create new figure
- `plt.savefig()` - Save figure to file
- `plt.show()` - Display plot
- `plt.close()` - Close figure

## 2. Matplotlib Axes Methods (`matplotlib.axes.Axes`)

```python
fig, ax = plt.subplots()
```

- `ax.plot()` - Line plot
- `ax.scatter()` - Scatter plot
- `ax.bar()` - Bar chart
- `ax.hist()` - Histogram
- `ax.boxplot()` - Box plot
- `ax.pie()` - Pie chart
- `ax.errorbar()` - Error bar plot
- `ax.fill()` - Fill area
- `ax.fill_between()` - Fill between curves
- `ax.imshow()` - Display image data
- `ax.contour()` - Contour plot
- `ax.contourf()` - Filled contour plot
- `ax.pcolor()` - Pseudocolor plot
- `ax.pcolormesh()` - Pseudocolor mesh
- `ax.hexbin()` - Hexagonal binning plot
- `ax.text()` - Add text
- `ax.annotate()` - Annotate points
- `ax.set_xlabel()` - Set x-axis label
- `ax.set_ylabel()` - Set y-axis label
- `ax.set_title()` - Set title
- `ax.set_xlim()` - Set x-axis limits
- `ax.set_ylim()` - Set y-axis limits
- `ax.set_xticks()` - Set x-axis ticks
- `ax.set_yticks()` - Set y-axis ticks
- `ax.grid()` - Show grid
- `ax.legend()` - Add legend
- `ax.colorbar()` - Add colorbar

## 3. Matplotlib Figure Methods (`matplotlib.figure.Figure`)

```python
fig = plt.figure()
```

- `fig.add_axes()` - Add axes to figure
- `fig.add_subplot()` - Add subplot to figure
- `fig.subplots()` - Create subplots
- `fig.savefig()` - Save figure
- `fig.canvas.draw()` - Redraw canvas
- `fig.canvas.flush_events()` - Flush GUI events
- `fig.tight_layout()` - Adjust layout
- `fig.set_size_inches()` - Set figure size
- `fig.gca()` - Get current axes
- `fig.gcf()` - Get current figure

## 4. Matplotlib Colormap Methods (`matplotlib.cm`)

```python
import matplotlib.cm as cm
```

- `cm.get_cmap()` - Get colormap
- `cm.ScalarMappable()` - Map scalar values to colors
- `cm.viridis()` - Viridis colormap
- `cm.plasma()` - Plasma colormap
- `cm.inferno()` - Inferno colormap
- `cm.magma()` - Magma colormap
- `cm.cividis()` - Cividis colormap

## 5. Matplotlib Style Methods (`matplotlib.style`)

```python
import matplotlib.style as style
```

- `style.use()` - Set style
- `style.available` - List available styles

## 6. Matplotlib Animation Methods (`matplotlib.animation`)

```python
import matplotlib.animation as animation
```

- `animation.FuncAnimation()` - Create animation from function
- `animation.ArtistAnimation()` - Create animation from artist frames
- `animation.PillowWriter()` - Save animation using Pillow
- `animation.FFMpegWriter()` - Save animation using FFmpeg
- `animation.ImageMagickWriter()` - Save animation using ImageMagick

## 7. Matplotlib Transforms Methods (`matplotlib.transforms`)

```python
import matplotlib.transforms as transforms
```

- `transforms.Affine2D()` - 2D affine transformation
- `transforms.Bbox()` - Bounding box transformation
- `transforms.IdentityTransform()` - Identity transformation
- `transforms.ScaledTranslation()` - Scaled translation
- `transforms.offset_copy()` - Offset transformation copy

---

This document provides a structured overview of key methods in `matplotlib`. For more details, refer to the [official documentation](https://matplotlib.org/stable/contents.html).
